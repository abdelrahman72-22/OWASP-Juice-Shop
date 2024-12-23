# Summary:

I found a Vulnerability in register page that allows me to signup with empty email and password

# Step To Reproduce:

1- visit https://juice-shop.herokuapp.com

2- Register a new account

3- inspect sign up element

4- delete `disabled="true"` from the the HTML element

5- press register

6- Go to login page and do the same in the login button

7- you are now signed with empty user

best regards,

naggar023, 0xSilent_Root

# Recommend Fix:

do server side validation
# Impact :

could cause some errors