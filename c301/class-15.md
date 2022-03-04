# Authentication

## What is OAuth

**What is OAuth?**

OAuth is an authorization framework

**Give an example of what using OAuth would look like.**

When you log on a website and you can use your google account as you login

**How does OAuth work? What are the steps that it takes to authenticate the user?**

1. First site connects to second site on behalf of the user, using OAuth
2. The second site generates a one time token and secret unique
3. First site gives token and secret to the users software
4. The client presents token and secret to authorization provider
5. If not authenticated to authorization provider, client may be asked to authenticate
6. User approves transaction at first site
7. User is given approved access token
8. user gives access token to first website
9. first site gives access token to second site

**What is OpenID?**
Similar to Oauth but without having to sign in or share login information 

<cite>What is OAuth,https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html</cite>

## Authorization and Authentication flows

**What is the difference between authorization and authentication?**

Authorization is the granting or denying of access to resources

Authentication process od providing if something is true

**What is Authorization Code Flow?**

Authorization Code Flow is the exchange of an Authorization Code for a token

**What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**

Similar to the Authorization Code Flow but adding the step of PKCE to introduce a secret by calling application that can be verified by the authorization server

**What is Implicit Flow with Form Post?**

The web app requests and obtains tokens through the front channel. This does not require secrets or more backend calls

**What is Client Credentials Flow?**

With M2M this flow authenticates and authorizes  the app rather then the user.

**What is Device Authorization Flow?**

For devices that have input constrains, the device asks users to use a link on the computer or smartphone to authorize a device

**What is Resource Owner Password Flow?**\

For trustworthy apps only, Resource Owner Password Flow requests the user Username and Password directly.

## Things I want to know more about
