# AnsibleProject

## Organize Your Repository

Setup dedicated repository for your ansible projects, which includes playbooks, roles, and inventories. You might want to have a structure like this:

.Directory Structure
```
.
├── .github/workflows
├── collections
│   └── requirements.txt
├── controller_configs
│   ├── all
│   ├── controller
│   ├── pah
│   └── eda
├── inventory.yml
└── controller_config.yml
```

## Setup

### Automation Content

1. Update the *rh-certified* **Remotes** 
   - Add your [Automation Hub Token](https://console.redhat.com/ansible/automation-hub/token)
   - Update the YAML requirements with below cellections
```yaml
collections:
  - name: ansible.platform
  - name: ansible.hub
  - name: ansible.eda
  - name: ansible.controller
```
![RH-Certified Remote](images/remote.png)

2. Under **Repositories** sync *rh-certified*
   
![RH-Certified Repository](images/repo.png)

### Automation Execution

1. Create **Credential** called *AAP Admin*
   
![AAP Credential](images/aap_cred.png)
## Function

[Red Hat Validated Collection infra.aap_configuration](https://github.com/redhat-cop/infra.aap_configuration)
