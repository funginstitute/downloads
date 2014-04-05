# Database Progress

## Known Issues
* classes for 1975 data mostly missing (~72,000) 
* titles truncated beyond 256 characters -- needs schema adjustment 
* location state field only allows 10 chars. Need to adjust to 20 chars.

## April 1, 2014

### Development

* moving ahead with fixing location schema so that locations can have better resolution
* updating database with grants, applications through April 1,2014

### Production

**grant**
* fixes pulled from development server. Now contains disambiguated inventor data

**application**
* fixes pulled from development server. Now contains fixed foreign keys and disambiguated inventor data

## March 31, 2014

### Development

**grant**
* inventor disambiguation finished

**application**

* inventor disambiguation finished

## March 27, 2014

### Development

**grant**
* awaiting joint grant/app inventor disambig

**application**
* ~~need to adjust claim foreign keys into the application table~~ DONE!
* awaiting joint grant/app inventor disambig

### Production

* awaiting most-recent inventor/assignee in location linking tables

**application**
* awaiting fixed foreign keys and app ids from apptest database


## March 14, 2014

### Development
* finished joint application/grant assignee disambig

**grant**
* awaiting joint grant/app inventor disambig

**application**
* need to adjust claim foreign keys into the application table
* awaiting joint grant/app inventor disambig


## March 12, 2014
-----------------
### Production
**grant**
* ~~finished backing up~~
* uploading to RDS database with fixed `inventor_location` links

## March 11, 2014
-----------------

### Production
**grant**
* finished backing up
* fixed error in flow where not all inventor records were linked to locations in the `inventor_location` table. 

**application**
* finished backing up

### Development
**grant**
* needs assignee disambiguation
* ~~needs location links to disambiguated records~~
* awaiting joint grant/app inventor disambig

**application**
* ~~needs location links to disambiguated records~~
* need to adjust claim foreign keys into the application table
* needs assignee disambiguation
* awaiting joint grant/app inventor disambig


## March 10, 2014
-----------------

### Production
**grant**
* currently backing up

**application**
* currently backing up

### Development
**grant**
* needs assignee disambiguation
* needs location links to disambiguated records
* awaiting joint grant/app inventor disambiguation

**application**
* need to adjust claim foreign keys into the application table
* needs assignee disambiguation
* needs location links to disambiguated records
* awaiting joint grant/app inventor disambiguation
