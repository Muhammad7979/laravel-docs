# Sociallite Laravel

###### **Some Pre-requisit**
- OAuth(Open auth)
    OAuth (Open Authorization) is an open standard protocol that allows secure authorization for third-party applications to access user data without sharing passwords. It is commonly used to let users log in to websites or apps using their accounts from services like Google, Facebook, or GitHub, while keeping their credentials safe.

    When you use OAuth to log in with services like Google, Facebook, or GitHub, the service typically sends back information such as:
    - User ID (unique identifier)
    - Name (full name or username)
    - Email address
    - Profile picture URL
    - Access token (used to access more data if needed)
    The exact information depends on the provider and the permissions you request. For example, Google may return the user's email and profile picture, while GitHub may return the username and avatar URL.

    Certainly! Here’s what happens behind the scenes when you use OAuth to log in with Google:

    1. **User Clicks "Login with Google":**  
        The user starts the login process by clicking the button in your app.

    2. **Redirect to Google:**  
        Your app redirects the user to Google’s OAuth authorization page, including information about what data your app wants to access.

    3. **User Grants Permission:**  
        The user logs in (if not already) and is asked to grant your app permission to access their Google data (like email and profile).

    4. **Google Redirects Back with Code:**  
        If the user approves, Google redirects the user back to your app with an **authorization code** in the URL.

    5. **App Requests Access Token:**  
        Your app sends the authorization code (plus your app’s credentials) to Google’s OAuth server to exchange it for an **access token**.

    6. **Google Responds with Access Token:**  
        Google sends back an access token (and sometimes a refresh token).

    7. **App Requests User Info:**  
        Your app uses the access token to request the user’s profile information from Google’s API.

    8. **Google Sends User Data:**  
        Google responds with the user’s data (like name, email, and profile picture), which your app can use to log the user in or create an account.

    **Summary:**  
        OAuth with Google is a secure, multi-step process that lets your app access user data without ever seeing their password.