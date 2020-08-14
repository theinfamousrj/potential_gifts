# Potential gifts
A MYSQL database for virtual gifts. It can be used as a model for games or even for serious wishlist apps.

### Initial dumb model

![alt text](https://github.com/bacloud14/potential_gifts/raw/master/data_model.PNG)

### DB

https://github.com/bacloud14/potential_gifts/raw/master/db.sql

#### Fields

##### generic_asset and assets tables
- description: description
- type: an asset can be:

   - productive like a machine, 
   - entertaining like a toy, 
   - raw like precious metals, 
   - information like any valuable information that is authentic or completely secret, 
   - symbolic like a love letter, 
   - assuring like a contract, 
   - other for anything other that these.
   
- ephemeral: wheather it is ephemeral like food or not
- expiration: only specified if it is ephemeral
- atomic: if it is valuable only if not devided like a computer keyboard
- valuable_exchange: if it still has value when given to others like real money
- unicode: unique just like id, but readible to identify all assets
- media: a picture link

##### user

user is just a subscribed user (technically for loggin but also for gaming).

##### possession

a possession is a one to many link so that a user can have many assets. Each entry is labeled by time to indicate the time of possessing an asset.

##### Note:

This is just my 0-version immagination of it, please feel free to open an issue and suggest any improvements.

### Dumb dump content

https://github.com/bacloud14/potential_gifts/raw/master/dump.sql



### todo

- Revise this 0 version and update the NodeJS model that will be used for Sequelize...
- NodeJS CRUD API to play with ?
- Make a web app game for virtual gifts ? For this we need some kind of virtual money units, to let users trade or exchange assets. A nice open source media package would be greate as you can imagine...
- Help wanted ! Propose any ideas ... This could be a huge amusement for teenageers.
