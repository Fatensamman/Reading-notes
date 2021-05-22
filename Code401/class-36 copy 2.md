# Application State with Redux

## What are the advantages of storing tokens in “Cookies” vs “Local Storage”

Local storage is vulnerable because it's easily accessible using JavaScript and an attacker can retrieve your access token and use it later.

The cookie is not accessible via JavaScript; hence, it is not as vulnerable to XSS attacks as localStorage.

- [LocalStorage vs Cookies: All You Need To Know About Storing JWT Tokens Securely in The Front-End](https://dev.to/cotter/localstorage-vs-cookies-all-you-need-to-know-about-storing-jwt-tokens-securely-in-the-front-end-15id#:~:text=Local%20storage%20is%20vulnerable%20because,attacks%20involving%20your%20access%20token.)

## Explain 3rd party cookies.

Third-party cookies are cookies that are set by a website other than the one you are currently on. For example, you can have a "Like" button on your website which will store a cookie on visitor's computer, that cookie can later be accessed by Facebook to identify visitor and see which websites he visited. Such cookie is considered to be a third-party cookie.

- [All you need to know about Third-Party Cookies](https://cookie-script.com/all-you-need-to-know-about-third-party-cookies.html#:~:text=Third%2Dparty%20cookies%20are%20cookies,see%20which%20websites%20he%20visited.)

## How do pixel tags work?

For marketing or media without a click event (such as navigating directly to a marketer’s website), click redirects cannot be used. In those cases, pixel tags (also known as pixels, 1x1 pixels, image tags or web bugs) are used instead. Pixel tags are typically single pixel, transparent GIF images that are added to a web page. Even though the pixel tag is virtually invisible, it is still served just like any other image you may see online. The trick is that the web page is served from the website’s domain while the image is served from the ad server’s domain. This allows the ad server to read and record the cookie with the unique ID and the extended information it needs to record.

- [COOKIES, TAGS AND PIXELS– TRACKING CUSTOMER ENGAGEMENT](https://resources.marketingeffectiveness.nielsen.com/blog/cookies-tags-pixels-tracking-customer-engagement#:~:text=Pixel%20tags%20are%20typically%20single,image%20you%20may%20see%20online.)

## Term

| Term | Definition |
| ------- | ----------------- |
|cookies| They are pieces of code that web servers use to put information on a user’s browser, and then retrieve that information at a later time for various uses. For example, YouTube sets a cookie on your browser to remember your username and volume settings so you don’t have to input those every time.|
|authorization|access rights/privileges to resources|
|access control|selective restriction of access to a place or other resource while access management describes the process. The act of accessing may mean consuming, entering, or using. Permission to access a resource is called authorization.|
|conditional rendering|Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them|

## Materials

[worlds easiest guide to redux](https://www.freecodecamp.org/news/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6/)

[testing reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)

[Redux Docs](https://redux.js.org/)