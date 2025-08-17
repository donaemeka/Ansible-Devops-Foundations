## Variables in Ansible


## What I Achieved
Automated server configurations using variables to:
✔ Eliminate hardcoded values in playbooks
✔ Reuse the same playbook across different environments (dev/stage/prod)
✔ Separate sensitive data from code (prep for Ansible Vault)

## Challenges I Solved

  ## Problem	                                              ## Solution
 
1. Playbook failed when variables were missing	  -   I Added validation: when: db_host is defined 

2. Mixed up variable precedence	                  -   Learned order: cli > playbook vars > inventory vars

3. Needed environment-specific configs	          -   Created separate prod_vars.yml, dev_vars.yml


## This lab taught me:

🔹 Maintainability: Change values in one place (vars file) vs. digging through playbooks

🔹 Security: Prepared me for Ansible Vault (next step for secrets)

🔹 Teamwork: Others can reuse my playbooks with their own variables