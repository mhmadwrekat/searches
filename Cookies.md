## Cookies

---

<!-- **How to get user preferences from cookies ?** -->

### What are Cookies?

Cookies are data, stored in small text files, on your computer.

When a web server has sent a web page to a browser, the connection is shut down, and the server forgets everything about the user.

Cookies were invented to solve the problem **how to remember information about the user**.

When a user visits a web page, his/her name can be _stored in a cookie._

Next time the user visits the page, the cookie "remembers" his/her name.

---

Cookies help us store the client-side data to enable a personalized experience for the website’s users. Cookies are sent with requests to the server and are sent to the client on response, hence the cookies data is exchanged with the server on every request. The servers could use the cookie data to send personalized content to users.

---

### Local storage VS Cookies?

1. **Storage Limit**
   - local Storage stores up to 10 megabytes
   - cookies provide a very restrictive and small storage capacity of 4 kilobytes.
2. **Accessibility**
   - local Storage could be accessed in any window or tab open on the browser for a website.
   - cookies are somewhat similar to local storage as they are accessible from any window or tab.
     Cookies could also be accessed on the server. Whenever we request the back-end server, all the cookies are also sent along. So they are also used for tasks related to authentication.
3. **Expiration**
   - Local Storage data never expires until you manually remove it, so in that sense, it could be very useful.
   - Cookies we can manually set the expiration date for them.

| Comparison                          | Cookies            | Local Storage |
| ----------------------------------- | ------------------ | ------------- |
| **Capacity**                        | 4KB                | 10MB          |
| **Browsers**                        | HTML 4 / HTML 5    | HTML 5        |
| **Accessible From**                 | Any window         | Any window    |
| **Expiration**                      | Manually set       | Never         |
| **Browser support**                 | Very high          | Very high     |
| **Supported data types**            | String only        | String only   |
| **Storage Location**                | Browser and server | Browser only  |
| **Editable and Blockable by users** | Yes                | Yes           |

---

---
