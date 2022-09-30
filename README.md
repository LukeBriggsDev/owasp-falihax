<img src="static/falihax.png" width="200" />

# Falihax OWASP Hackathon

## Found Issues
- App is run in debug mode
- No login brute force limit
- No password complexity requirement
- No logging for secuirty events (login, registration, password failure)
- Vulnerable to SQL injection by not using prepared statements
	- Fixed [here](commit/51757ee526e42201e4ec316e64c3f4a95ff36c19) and [here](commit/d9f2ac0c22a95c44c5df5084f0fd392ae63ac71a)
- Passwords not hashed and salted (uses weak rot13)
	- Fixed [here](commit/d86c1663876afca48d6d15598795b3b04f9ea873)
- Sort code and account number generated using non CSPRNG, might lead to an attacker being able to guess a user's account details
	- Fixed [here](commit/85dcdad0e35cc297a65dbf6802e8e0f93cd5c253)
- Any user can visit the admin page
	- Fixed [here](commit/6dff0feb13d255abe5e8661669b6fe43003ac353)
- Any user can access any other user's transaction page
	- Fixed [here](commit/89015d8ab789c326cc7866cc23ac684a8e69b986)
- Correct name for an account is only checked at the client side
	- Fixed [here](commit/43c60628f79757080b063ebcdbb4b5e0df9f3dad)
- Transactions can have a negative value, allowing anyone to pay themselves money from any account
	- Fixed [here](commit/d0cf14043d5204cdcedc32bcb47a614106d9b8d3)
- The validation for credit score is only validated at the client side
	- Fixed [here](commit/58b3f362e5885cf8f287c91a06b1d7af3d96737a)

## Premise
Falihax is a brand new, 100%* real and secure banking company. Last year, they
contracted a group of computer science students to build a website for them -
unfortunately, none of these students
were [CyberSoc](https://cybersoc.org.uk/?r=falihax) members and so didn't know
how to build a web app securely.

Recently, they have experienced a number of
attacks on their website. They are insistent that their website is very safe and
not at all vulnerable, but nevertheless they have asked you to help them improve
their security!

**percentage expressed in binary. 4% margin of error.*

## Task
Download or fork this repository, and try to find as many security vulnerabilites
as possible and fix them!

## Competition

[Click here](https://forms.office.com/r/hza2ZDWt02) to submit your entry when
you have finished, to enter the competition! Competition rules and prizes are
displayed on the form.

## Need help?
Just ask us as we move around the room, or alternatively you can ask on our
cyber help channel on our [Discord server](https://cybersoc.org.uk/discord).
To access it, just join and message us to say you're in the hackathon, and you
will be given access to the cyber help and resources channels!

*All companies, content and people portrayed in this work
are fictitious or parodic in nature. No association with actual people or
companies is intended or should be inferred.*
