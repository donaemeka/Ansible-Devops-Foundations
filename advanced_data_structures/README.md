# Scalable Automation with Lists & Dictionaries  

## Why This Matters  

Manual package management doesn't scale. This lab demonstrates:  

✅ Installing 10+ packages with **3 lines of YAML**  

✅ Handling service name variations (e.g., `mysql` vs `mariadb-server`)  

✅ Structuring complex configs cleanly  



## Lessons Learned

- Idempotency: Why state: present matters

- Real-World Adaptation: Ubuntu vs CentOS package names

- Error Handling: Using ignore_errors with block/rescue


## Validation

- systemctl status apache2 mysql  # Verify services 

- dpkg -l | grep -E 'apache|mariadb'  # Check packages  