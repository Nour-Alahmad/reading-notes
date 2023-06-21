# JSON Web Token

## Intro to JWT

### What is a JSON Web Token (JWT)?

A JSON Web Token (JWT) is a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be used for authentication, authorization, information exchange, and other purposes.

### When should we use JSON Web Tokens?

JWTs are a good choice for applications that need to securely transmit information between parties. They are especially well-suited for applications that need to be able to verify the identity of the sender and the integrity of the information. For example, JWTs can be used to:

- Authenticate users in a single sign-on (SSO) system
- Exchange information between a client and a server
- Verify the authenticity of a message

### Claims are expected in which structural component of a JWT?

Claims are expected in the payload structural component of a JWT. The payload is a JSON object that contains the claims, which are statements about the subject of the token. The claims can be used to represent any type of information, such as the user's identity, their authorization level, or the expiration time of the token

---

## Are JWTs Secure?

### If I get a JWT and I can decode the payload, how can we call that secure?

A JWT is secure because it is signed with a secret key. This means that anyone who tries to decode the payload will need to know the secret key. If you can decode the payload, it means that you know the secret key, which means that you are the intended recipient of the JWT.

### If sending a JWT, what must sender and receiver both know?

The sender and receiver must both know the following:

The secret key used to sign the JWT
The format of the JWT
The algorithms used to encode and decode the JWT

### Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

To send and receive concatenated content and secret securely, you can use a secure messaging service like Signal or WhatsApp. These services use end-to-end encryption, which means that only the sender and receiver can read the messages.

You can also use a public key infrastructure (PKI) to send and receive concatenated content and secret securely. PKI uses a public key and a private key to encrypt and decrypt messages. The public key is known to everyone, but the private key is only known to the sender and receiver.

Here is an analogy that you can use to explain this to a non-technical recruiter:

Imagine that you want to send a secret message to a friend. You could write the message on a piece of paper and seal it in an envelope. You would then give the envelope to your friend, who would be able to open it and read the message because they have the key to the envelope.

With PKI, the piece of paper is the concatenated content, the envelope is the encryption, and the key to the envelope is the private key.

---

## How to use JWT

### Why use JWT?

 JWTs are often used as authorization tokens in web applications.it is very small, which makes them ideal for transmitting over HTTP headers and JWTs contain all the information they need to be verified, which means that they don't need to be stored in a database. it also can be signed or encrypted, which makes them tamper-proof.

### JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

Imagine I want to send a secret message to my friend. I could write the message on a piece of paper and seal it in an envelope. Then, I could give the envelope to my friend, who would be able to open it and read the message because he has the key to the envelope.
JWTs are similar to this. They are a way of sending a secret message, but instead of using an envelope, they use a JSON object. The JSON object is compact and self-contained, which means that it can be easily transmitted over HTTP headers.

### What are the three components (the structure) of a JWT signature?

The three components of a JWT signature are:

- Header: The header contains the type of token, the signing algorithm, and the token's claims.
- Payload: The payload contains the claims, which are the data that is being transmitted.
- Signature: The signature is used to verify the authenticity of the token.
The header and payload are encoded using Base64url encoding. The signature is created using a cryptographic algorithm, such as HMAC-SHA256 or RSA.