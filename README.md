# devcontainer-ansible
VSCode devcontainer for Ansible development

## Pre-requisites Windows

1. Install Podman Desktop from <https://podman-desktop.io/>. Configure the Podman Machine to use WSL2 and enable User mode networking.
2. Configure VS Code to use Podman instead of Docker (`settings.json`) and disable forwarding of WSL services:
   ```json
    "dev.containers.dockerPath": "podman",
    "dev.containers.forwardWSLServices": false,
   ```
3. Open the repository in VS Code and click on the "Reopen in Container" button in the notification that appears at the bottom right corner of the window.

## Pre-requisites Linux

1. Install Podman using your favorite package manager.
2. Open the repository in VS Code and click on the "Reopen in Container" button in the notification that appears at the bottom right corner of the window.

## Run Ansible

Execute the following command to run the included Ansible playbook:

```shell
$ ansible-playbook playbook.yaml
```
![image](https://github.com/user-attachments/assets/9efeb925-8085-4405-a157-4334b1ceff62)
