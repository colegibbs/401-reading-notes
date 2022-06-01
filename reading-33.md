# Reading 33: Authentication and Production Server

## [JSON Web Tokens](https://jwt.io/introduction/)

- a way to send json securely
- signed with keys to encrpyt and decrpyt based on the sender and reciever
- Use cases:
  - authorization: given JWT as login and carried with you through site to give access
  - information exchange: secure way to send info and can see if info has been tampered with
- structure: Header.Payload.Signature
- Header
  - signing algorithm and type 
- Payload
  - contains claims about user
  - Registed, public, and private claims
  - registered claims
    - not madatory
    - predefined
  - public claims
    - custom claims
    - to avoid collision should be defined in the IANA JSON Web Token Registry or be defined a sa url that contains a collison resistant namespace
  - private claims
    - the info between parties that ar not public or registered claims
- Signature
  - sign the entire thing
  - signature used to verigy message wasn't change along the way and the sender is who they say they are
- should not keep tokens longer than required
- don't send too large of tokens through the headers
- use a differnet method if too big
- don't push secret info within the token
- benefits
  - compact
  - simple
  - mapped easily

## [DRF JWT Authentication](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)

- token should be included in all requests
- installation and set up
  - pip install djangorestframework_simplejwt
  - settings.py
    - REST_FRAMEWORK authentication
  - urls.py
    - token path and token refresh path
  - obtain token
  - token lasts five minutes
  - to get a new token refresh the token refresh endpoint
- refresh token allows for speed by removing uneeded steps
- refresh toekn allows for better security

## [Django Runserver Is Not Your Production Server](https://build.vsupalov.com/django-runserver-in-production/)

- runserver command is not meant for production
- using a WSGI server and more specifically a Gunicorn server for deployment; server: Nginx
- function is called when the request comes in and passes that info to function and then responds with corrently formated data

## Bookmark

- [JWT with DRF](https://www.youtube.com/watch?v=Fhcn2qx-4VQ)
- [Gunicorn](https://gunicorn.org/)
- [Django Migrations Primer](https://realpython.com/django-migrations-a-primer/)