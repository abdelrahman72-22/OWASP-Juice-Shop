Summary:
i found reflected xss in search input and i used the payload <img src=x onerror=alert(document.cookie)>  which would lead to steel cookies, so lead to Account takover

Step To Reproduce:
1-visit https://juice-shop.herokuapp.com
2-go to search input
3-inject the payload <img src=x onerror=alert(document.cookie)>
4-observe alert of the cookie in the page

best regards,
0xSilent_Root

Recommend Fix:
1-Filter the input of search by applying input length restirictions
2-Escaping HTML to prevent xss attacks in search results

Impact :
lead to account takeover
