# Summary:

i found sql injection in login page and i used the payload **admin' OR 1=1 --**  which would lead to steel admin account , so lead to Account takover

# Step To Reproduce:

1-visit https://juice-shop.herokuapp.com

2-go to login page

3-inject the payload **admin' OR 1=1 --**

4-you can login as admin

best regards,

0xSilent_Root , naggar023

# Recommend Fix:

1-use parameterized queries or prepared statments to seperate SQL logic from user input

2-Validate input to ensure it matches the expected format. for example, username should only contain alphanumirc characters.

# Impact :

lead to account takeover like admin