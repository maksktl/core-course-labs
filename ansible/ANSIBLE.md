### **Result of ansible-playbook playbooks/dev/main.yml --diff**

```
TASK [web_app : Ensure /etc/docker/ directory exists.] *********************************************************************************************************************
skipping: [vm]

TASK [web_app : Configure Docker daemon options.] **************************************************************************************************************************
skipping: [vm]

TASK [web_app : Ensure Docker is started and enabled at boot.] *************************************************************************************************************
ok: [vm]

TASK [web_app : Ensure handlers are notified now to avoid firewall conflicts.] *********************************************************************************************

TASK [web_app : include_tasks] *********************************************************************************************************************************************
included: /Users/nurbakzh/Downloads/labs/DevOps-Nurba/ansible/roles/nurba/tasks/docker-compose.yml for retakeVM

TASK [web_app : Check current docker-compose version.] *********************************************************************************************************************
ok: [vm]

TASK [web_app : set_fact] **************************************************************************************************************************************************
ok: [vm]

TASK [web_app : Delete existing docker-compose version if it's different.] *************************************************************************************************
skipping: [vm]

TASK [web_app : Install Docker Compose (if configured).] *******************************************************************************************************************
skipping: [vm]

TASK [web_app : Get docker group info using getent.] ***********************************************************************************************************************
skipping: [vm]

TASK [web_app : Check if there are any users to add to the docker group.] **************************************************************************************************

TASK [web_app : include_tasks] *********************************************************************************************************************************************
skipping: [vm]

TASK [web_app : Stop services] *********************************************************************************************************************************************
skipping: [vm]

TASK [web_app : Remove directory] ******************************************************************************************************************************************
skipping: [vm]

TASK [web_app : Create directory] ******************************************************************************************************************************************
ok: [vm]

TASK [web_app : Crete docker-compose.yml] **********************************************************************************************************************************
ok: [vm]

TASK [web_app : Run docker-compose] ****************************************************************************************************************************************
ok: [vm]

PLAY RECAP *****************************************************************************************************************************************************************
vm                   : ok=19   changed=0    unreachable=0    failed=0    skipped=16   rescued=0    ignored=0```
```