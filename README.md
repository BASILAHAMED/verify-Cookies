
# Cookie Verification with Selenium

### Verify Cookies 🔐

This script utilizes Selenium to interact with a web page, facilitating the logging in and logging out processes while checking cookies before and after these actions. This code is instrumental in understanding how a website's cookies evolve as a user undergoes the login and logout processes. Cookies often store session-related information, and their values might change dynamically based on user interactions with the website.

## Code Breakdown

**Initialization:**
- Sets up a WebDriver using Selenium tailored for Chrome.
- Implicitly waits for a maximum of 10 seconds for elements to appear on the page.

**`fetch_cookies()` Method:**
- Opens the specified URL (https://www.saucedemo.com/).
- Maximizes the browser window.
- Prints the cookies before the login process.
- Enters a username and password, then clicks the login button.
- Prints the cookies after the login process.
- Clicks on the burger menu and logs out.
- Prints the cookies after the logout process.

**`shutdown()` Method:**
- Closes the browser session.

## Getting Started

To get started with cookie verification using Selenium, follow these steps:

1. Clone this repository to your local machine.
   ```bash
**   git clone https://github.com/your-username/verify-Cookies.git**

2. Navigate to the project directory.
**cd cookie-verification-selenium**
Install the required dependencies using pip.

3. Install the required dependencies using pip.
**pip install -r requirements.txt**
Run the script.

4. Run the script.
**python verify_cookies.py**

### Output ⭐⭐⭐
```
cookies before login = []
cookies after login = [{'domain': 'www.saucedemo.com', 'expiry': xxxxxxxxx, 'httpOnly': False, 'name': 'session-username', 'path': '/', 'sameSite': 'Lax', 'secure': False, 'value': 'visual_user'}]
cookies after logout = []```
