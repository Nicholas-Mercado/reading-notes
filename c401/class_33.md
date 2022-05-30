# Authentication & Production Server

## JSON Web Tokens

JSON Web Token (JWT) - a self-contained way for securely transmitting information between parties as a JSON object

JWTs can be signed with:

- HMAC algorithm

- RSA or ECDSA pair

### What is the JSON Web Token structure?

- Header
  - consists of two parties
    - type
    - signing algorithm

    ex:

```py
        {
  "alg": "HS256",
  "typ": "JWT"
}
```

- Payload

    Contains claims:

  - Registered claims
    - set of predefined claim
      - Are not mandatory
        - iss (issuer)
        - exp (expiration time)
        - sub (subject)
        - aud (audience)
        - etc..
  - Public claims
    - Can be defined at will
  - Private claims
    - Custom claims both parties agree on using
  
- Signature
  - How to create a Signature

ex:
```py
HMACSHA256(
  base64UrlEncode(header) + "." +
  base64UrlEncode(payload),
  secret)
```
  

