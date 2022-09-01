# Authentication and Production Server

## JSON Web Tokens

JSON Web Tokens, or JWT is a secure way to transmit information between two parties that is digitally signed.

Authorization is the most common scenario for using JWT. Once a user is logged in, they will send all requests with that JWT and will get to see different information based on the authorization of that token.

Because they are signed, JWT are a good way to transmit information between parties due to the fact that that signature guarantees both parties are who they say they are.

Parts of a JWT: Header, Payload, Signature

* Header: consists of two parts: the type of the token, and the signing algorithm used.

* Payload: contains the claims. Claims are statements about the user and additional data.

* Signature: is the part of the JWT that confirms the information wasn't modified along the way.

## Production Server

The servers we have been running are not yet cleared for a production level.

## Things I want to know more about:

* I don't really understand the difference between a production and a non-production server. I understand that there is some amount of security that is heightened in the production level, but that is still fuzzy to me at this point.
