---
title: 'Rolling your own auth'
date: 2024-11-12
draft: true
showtoc: true
ShowReadingTime: true
author: Alex Kellermann
summary: Rolling my own Auth server to learn about Auth.
tags: [Security, Auth, golang, html, react, Google, OIDC, SAML, Oauth]
cover:
    image: '/img/auth/auth.webp'
---

# Disclaimer:
This isn't rolling your own crypto: which you obviously shouldn't do. Rolling your own auth means building on top of the shoulders of giants, following a well paved path and not shelling out hundreds of thousands of dollars to a service like auth0 to handle it for you.

# Why am I doing this?
To Learn

## The plan
- Learn how to write AuthN and AuthZ services.
- Learn how to handle things like sessions and cookies on the web.

## What isn't a concern.
- Scaling issues.
- Flexibility.

# Creating Username and Password-based logins
This is the defacto standard for applications. Even though more and more websites are offering single sign on through OIDC, I think it's important to still offer username/password login. Users are more familiar with it than technologies like Passkeys.


Using ArgonID / maybe bcrypt

# Creating a small front end
{{< figure src="/img/auth/loginpagev1.png" class="normal" >}}

# The browser is your ~enemy~ friend!
While prototyping, the browser will fight you tooth and nail if you don't follow best practices. This was my experience testing in both Safari and Google Chrome. As a security engineer, I think this is fantastic. Ultimately it made me decide against choosing a web server like NGINX or some third party library in golang to handle things like setting cookies or obfuscating tasks like handling sessions or [CSRF](https://owasp.org/www-community/attacks/csrf).

## Running into CORS issues.

1. Authn service on localhost:8081
2. Frontend HTTP service on localhost:8082

Sending credentials to a different origin requires setting the headers:
    - "Access-Control-Allow-Credentials"
    - "Access-Control-Expose-Headers"

# Adding OIDC w/ Google
I wouldn't bother adding other providers except maybe sign in with Apple. OIDC is built on top of Oauth, so you'll need an Oauth clientID and client Secret
Golang doesn't have a nice wrapped around OIDC, only oauth, so you'll need to use an external librayr to hide the complexity of doing OIDC yourself. I chose this one by CoreOS: https://github.com/coreos/go-oidc/tree/v3/example

```goat
Auth Frontend ---> other thing
```