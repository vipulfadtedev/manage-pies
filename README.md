# manage-pies
This project help me manage my pies... [WIP]<br>
Currently it doest upgrade pies and can reboot em.

## Commands:
1. Upgrade:<br>
    1. All : <br>
    ```ansible-playbook -i inventory.yaml --extra-vars "hosts=all" playbook-upgrade.yaml```
    2. Util : <br>
    ```ansible-playbook -i inventory.yaml --extra-vars "hosts=util" playbook-upgrade.yaml```
    3. Cluster : <br>
    ```ansible-playbook -i inventory.yaml --extra-vars "hosts=cluster" playbook-upgrade.yaml```

2. Reboot<br>
    ```ansible-playbook -i inventory.yaml --extra-vars "hosts=all" playbook-reboot.yaml```
