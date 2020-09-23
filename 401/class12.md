# OAuth

1. **Why is authentication important?**

Because it enables organizations to keep their networks secure by permitting only authenticated users.

2. **Why should we be careful about storing a user’s password?**

When you store a user's password, you must ensure that you have it secured in such a way that if your data is compromised, you don't expose your user's password.

3. **What is the difference between hashing and encryption?**

Encryption is a two-way function; what is encrypted can be decrypted with the proper key. Hashing, however, is a one-way function that scrambles plain text to produce a unique message digest. With a properly designed algorithm, there is no way to reverse the hashing process to reveal the original password.

4. **What is the difference between encryption and encoding?**

Encoding is for maintaining data usability and can be reversed by employing the same algorithm that encoded the content, i.e. no key is used. Encryption is for maintaining data confidentiality and requires the use of a key (kept secret) in order to return to plaintext.

5. **What is a token used for?**
A token is used to make security decisions and to store tamper-proof information about some system entity. While a token is generally used to represent only security information, it is capable of holding additional free-form data that can be attached while the token is being created.

## Vocabulary Terms
### Authentication
Authentication is the process of recognizing a user's identity.
### Authorization
Determines what you can do/if the client has permissions. 
### Encryption
Is the method by which information is converted into secret code that hides the information's true meaning.
### Hashing
Is the process of converting a given key into another value.
### Session
Keep users from having to login multiple times.
### Cookie
Cookies allow users to be recognized within a website so any page changes or item or data selection you do is remembered from page to page.
### Token
In general, a token is an object that represents something else, such as another object (either physical or virtual).
### Basic Auth
Is a simple authentication scheme built into the HTTP protocol.
### Encoding
Is to transform data so that it can be properly (and safely) consumed by a different type of system, e.g. binary data being sent over email, or viewing special characters on a web page. The goal is not to keep information secret, but rather to ensure that it's able to be properly consumed.
### Secret
Used by the OAuth Client to Authenticate to the Authorization Server.
### Cryptography
Is the study of secure communications techniques that allow only the sender and intended recipient of a message to view its contents. ... When transmitting electronic data, the most common use of *cryptography* is to encrypt and decrypt email and other plain-text messages.
