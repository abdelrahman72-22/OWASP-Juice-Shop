# Summary:

I found Broken Access Control Vulnerability on shopping cart that allows me to view the shopping cart of another user by editing bid in session storage

# Step To Reproduce:

1-visit https://juice-shop.herokuapp.com

2-press `your basket` button

3- open your browser dev tools

4- go to storage tab

5- open session storage and edit bid to any value

6- refresh the page

7- see how the cart changing to give you another user cart

best regards,

naggar023, 0xSilent_Root

# Recommend Fix:

- Use Server side authorization 
- use Json Web token (JWT)
# Impact :

viewing cart of another user
