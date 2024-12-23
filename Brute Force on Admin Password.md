# Summary:

i can bypass admin account by guessing the password 

# Step To Reproduce:

1-login the admin account with email  admin@juice-sh.op and write any password

2-go to burpsuite and click intercept is off  to make it on and click on login in owasp juice shop 

3-send the request to intruder and select the password you write => click add =>  paste the top 100 password from github 

4-click on start attack and monitor the status code , if see 200 OK then the password is correct 

best regards,

0xSilent_Root , naggar023

# Recommend Fix:

1-Lock for 15 minutes after 5 failed attempts (Rate limit)

2-Add CAPTCHA (e.g., Google reCAPTCHA) after multiple failed login attempts to prevent automated attacks.

# Impact :

lead to account takeover like admin