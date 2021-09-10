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

2. Update firmware<br>
    ```ansible-playbook -i inventory.yaml --extra-vars "hosts=all" playbook-update-firmware.yaml```
	
3. Reboot<br>
    ```ansible-playbook -i inventory.yaml --extra-vars "hosts=all" playbook-reboot.yaml```

4. Start collecting stats <br>
    ```ansible-playbook -i inventory.yaml --extra-vars "hosts=all" playbook-stats-git.yaml```	
	
5. Rotate Logs<br>
    ```ansible-playbook -i 10.0.0.4, playbook-rotate-logs-git.yaml```	
	
6. Install zabbix agent
	```ansible-playbook -i inventory.yaml --extra-vars "hosts=other-than-zabbix" zabbix-agent-install.yaml```