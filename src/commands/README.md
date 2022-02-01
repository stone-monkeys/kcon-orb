# Commands

Easily add and author [Reusable Commands](https://circleci.com/docs/2.0/reusing-config/#authoring-reusable-commands) to the `src/commands` directory.

Each _YAML_ file within this directory will be treated as an orb command, with a name which matches its filename.

View _[install.yml](./install.yml)_ example.

```yaml
description: >
  This command installs kconnect to your execution environment

steps:
  - run:
      name: Install Kconnect
      command: | 
        curl -fsSL -o install-kconnect.sh https://raw.githubusercontent.com/fidelity/kconnect/main/scripts/install-kconnect.sh
        chmod 700 install-kconnect.sh
        ./install-kconnect.sh
        cd kconnect 
        sudo cp kconnect /usr/local/bin
        sudo cp aws-iam-authenticator /usr/local/bin
        sudo cp kubectl /usr/local/bin
```

## See:
 - [Orb Author Intro](https://circleci.com/docs/2.0/orb-author-intro/#section=configuration)
 - [How to author commands](https://circleci.com/docs/2.0/reusing-config/#authoring-reusable-commands)
