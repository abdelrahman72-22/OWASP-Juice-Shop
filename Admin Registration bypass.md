# Summary:

i can create account with admin privileges 

# Step To Reproduce:

1-go to owasp juice shop and register an account 

2- write any email and password and click register

3-go to burpsuite and click intercept is off  to make it on . click on register in owasp juice shop to intercept the request 

3-modify the request and add "role"="admin" in request in burp and right click  do intercept => response to this request => forward => go to refresh page 


best regards,

0xSilent_Root , naggar023

# Recommend Fix:

1- Sanitize and validate all inputs on both the client and server sides.

2-Reject unexpected characters, especially in critical fields like usernames and passwords.

3-Use allowlists (e.g., only alphanumeric characters for usernames).

# Impact :

- Attackers may register as an admin without proper authorization.
- They gain access to sensitive areas of the application intended only for trusted users.