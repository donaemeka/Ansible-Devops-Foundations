# Apache Automation  

## What I Learned  
- Fixed `apt` lock issues with `update_cache: yes`  
- Service names ≠ package names (`apache2` vs `httpd`)  
- How to verify with `curl http://localhost`  

## Key Code  
yaml
- name: Ensure Apache runs after reboot  
  service:  
    name: apache2  
    enabled: yes  