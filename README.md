# Trainning
### Linux Commands
* For Basic Commands of Linux terminal read [terminal.md](https://github.com/dipen-atharva/Trainning/blob/main/terminal/terminal.md)

--- 
### Authentication 

* Authentication is a process in which the credentials provided are compared to those on file in a database of authorized users' information on a local operating system or within an authentication server. If the credentials match, the process is completed and the user is granted authorization for access.

### Authorization

* Authorization is the process of giving someone permission to do or have something.


*Authentication is the first step of a good identity and access management process. Authorization always takes place after authentication. Authentication is visible to and partially changeable by the user. Authorization isn't visible to or changeable by the user.*


### Ways to achieve authentication

* Session Based Authentication - Utilizes browser Cookies along with backend "Sessions" to manage logged-in and logged-out users.

* JWT Authentication - A stateless authentication method where a JSON Web token (JWT) is stored in the browser (usually localStorage). This JWT has assertions about a user and can only be decoded using a secret that is stored on the server.

* OAuth and OpenID Connect Authentication - A modern authentication method where an application uses "claims" generated from other applications to authenticate its own users. In other words, this is federated authentication where an existing service (like Google) handles the authentication and storage of users while your application leverages this flow to authenticate users.

### 1. Cookie based Authentication

- Authentication is the process of exchanging user credentials for a piece of unique identification.

- When you log in to a web application, your browser will receive a cookie from its application’s server, and the browser will store it and send that cookie with each subsequent request to verify that requests come from the same user.

- Step by step
    1. User login to the application using credentials.
    2.  Server validates the credentials and creates a session in the database.
    3. Server responds with the cookie to the browser by including it in the Set-Cookie header.
    4. Browser stores the Cookie in storage and sends it with subsequent requests.
    5. When the user logout, the server will delete the session from the database.

### 2. Cookie based Authentication

- Token-based authentication was introduced to address several shortcomings of the Cookie-based approach.

- When you log in to a web application, the server will verify your credentials and send an encrypted token to the browser. Then the browser will store this token and can be added to the authorization header of future requests.

- JSON Web Token (JWT) is the most used open standard in token-based authentication.

- Step by step
    1. User login to the application using credentials.
    2. The server verifies the credentials, generates a token and signs it with a secret key, and sends it back to the browser.
    3. Store the token in the browser storage and add to subsequent requests using JavaScript.
    4. When the user logout, you need to delete the token from its storage manually.


### 3. OAuth

- OAuth is an open-standard authorization protocol or framework that provides applications the ability for “secure designated access.” For example, you can tell Facebook that it’s OK for ESPN.com to access your profile or post updates to your timeline without having to give ESPN your Facebook password. This minimizes risk in a major way: In the event ESPN suffers a breach, your Facebook password remains safe.

- OAuth doesn’t share password data but instead uses authorization tokens to prove an identity between consumers and service providers. OAuth is an authentication protocol that allows you to approve one application interacting with another on your behalf without giving away your password.
