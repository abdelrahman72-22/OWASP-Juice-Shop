# Summary:

i can enumarate the directories in owasp juice shop and find directiory belongs to admin  

# Step To Reproduce:

1-use the ffuf tool to find directories

2-  write ffuf -u http://localhost:3000/FUZZ -w common.txt

best regards,

0xSilent_Root 

# Recommend Fix:

1- Avoid using predictable or default paths for sensitive resources.

2-Use a WAF to detect and block automated enumeration attempts.

3-Limit the number of requests from a single IP to prevent automated enumeration

# Impact :

Access to sensitive resources like admin (`/administration`).
Attackers can gain unauthorized access to functionalities or sensitive information that should be protected.