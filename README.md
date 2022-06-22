# ![GA Logo](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Auth Research Lab

---

Authentication is a complex and exciting topic that involves using many of the concepts we've already studied as well as several new ideas. 

An authentication system allows the registration / signup of new users and allows those users to sign in. It has to be able to identify each user and keep their information private and secure.

Being able to develop secure user login systems is in fact a whole career and life path in and of itself, but understanding the broad concepts of **Auth** is critically import for all developers. 

Describing auth flow and understanding key terms are very common **interview questions** for junior developers, so lets take some time to research and understand auth and the related concepts.

## Setup

Fork and clone this repository and answer the questions as you research directly in the README. You do not have to pull request and submit this lab, but you will want to have it on hand for reference in the future. 

## Auth Concepts Worksheet

#### Define the following

1. *Authentication*

Proving that a user is valid -- credentials match

1st step

visible and changeable by user

2. *Authorization*

The rules that allow a user to perform actions -- permissions

2nd step

is not visible or changeable to user

3. Explain how *authentication* and *authorization* are related but distinct concepts.

Authentication is used to verify that users really are who they represent themselves to be. 
Authorization is then used to grant the user permission to access different levels of information and perform specific functions, depending on the rules established for different types of users.

5. *Sessions vs Token based auth*

The main difference is session-based authentication of the connection stores the authentication details. -- cookies

possessing a token is the only thing that a user needs to have their requests authorized by the server, which must only verify a signature. The token is secure to use because it cannot be tampered with.

6. *json web token (also know as a jwt)*

JWT contains encoded JSON objects, including a set of claims. JWTs are signed using a cryptographic algorithm to ensure that the claims cannot be altered after the token is issued.

a claim may assert who issued the token, how long it is valid for, or what permissions the client has been granted.

7. *Encoding, encryption and hashing* along with the uses for and differences between the three

Encoding is not used to security purpose. It is a technique in which the data is transformed from one format into another, so that it can be understood and consumed by different systems

Encryption makes the data unreadable and difficult to decode for an attacker and prevents it to be stolen. Using the key, the data is Encrypted at the sender’s end and using the same or different key, the data is Decrypted at the receiver's end

Hashing is a technique to ensure the integrity of the data by converting it into a fixed-length string.

8. *oAuth* (pronounced oh-Auth)

OAuth (pronounced “oh-auth”) is a technological standard that allows you to share information between services without exposing your password.

#### Explore and then describe the following npm packages:

1. [bcrypt](https://www.npmjs.com/package/bcrypt)

A library to help you hash passwords.

2. [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken)

creates a JWT

3. [passport](https://www.npmjs.com/package/passport)
    * also describe what a *strategy* is in the context of this npm package


purpose is to authenticate requests. you provide Passport a request to authenticate, and Passport provides hooks for controlling what occurs when authentication succeeds or fails.

---

## Licensing
1. All content is licensed under a CC-BY-NC-SA 4.0 license.
2. All software code is licensed under GNU GPLv3. For commercial use or alternative licensing, please contact legal@ga.co.