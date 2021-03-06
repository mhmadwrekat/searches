# Cookies

---

<!-- **How to get user preferences from cookies ?** -->

## What are Cookies?

Cookies are data, stored in small text files, on your computer.

When a web server has sent a web page to a browser, the connection is shut down, and the server forgets everything about the user.

Cookies were invented to solve the problem **how to remember information about the user**.

When a user visits a web page, his/her name can be _stored in a cookie._

Next time the user visits the page, the cookie "remembers" his/her name.

---

Cookies help us store the client-side data to enable a personalized experience for the website’s users. Cookies are sent with requests to the server and are sent to the client on response, hence the cookies data is exchanged with the server on every request. The servers could use the cookie data to send personalized content to users.

---

## Local storage VS Cookies?

![Local storage VS Cookies](https://res.cloudinary.com/academind-gmbh/image/upload//v1/academind.com/content/tutorials/localstorage-vs-cookies-xss/localstorage-vs-cookies-xss)

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

## **How cookies can be used to preferences?**

1. Do not use unnecessary content

   - What has been previously read by a user can be collected and then shown to him, And some topics that the user did not care about should not be shown to him in the next time.
   - And we can put his preference at the top of the site and others at the end .

2. does he open any video !!

   The user can be tracked in the event that he plays the video, a larger amount of the video will be shown to him in the next time and in top of website, and vice versa

3. does he open any vioces !!

   The user can be tracked in the event that he plays the voices, a larger amount of the voices will be shown to him in the next time and in top of website, and vice versa

---

## Reference

1. [Article](https://www.xenonstack.com/insights/local-vs-session-storage-vs-cookie)

2. [Youtube Video](https://www.youtube.com/watch?v=sovAIX4doOE&list=LL&index=1&t=517s)

3. [Stack overflow](https://stackoverflow.com/questions/7799728/localstorage-vs-cookies-performance)

---
