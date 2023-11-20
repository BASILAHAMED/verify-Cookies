### Verify Cookies

Using Selenium to interact with a web page, log in, and check cookies before and after the login/logout process. This code is particularly useful for understanding how the website's cookies change as a user goes through the login and logout processes. Cookies often store session-related information, so their values might change as the user interacts with the website.
### Code Breakdown
**Initialization:**
Sets up a WebDriver using Selenium for Chrome.
Implicitly waits for a maximum of 10 seconds for elements to appear on the page.

**get_cooky() method:**
Opens the specified URL (https://www.saucedemo.com/).
Maximizes the browser window.
Prints the cookies before login.
Enters a username and password, then clicks the login button.
Prints the cookies after login.
Clicks on the burger menu and logs out.
Prints the cookies after logout.

**shutdown() method:**
Closes the browser session.

### Output
```
cookies before login = []
cookies after login = [{'domain': 'www.saucedemo.com', 'expiry': xxxxxxxxx, 'httpOnly': False, 'name': 'session-username', 'path': '/', 'sameSite': 'Lax', 'secure': False, 'value': 'visual_user'}]
cookies after logout = []
```
