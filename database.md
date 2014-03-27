# Database Progress

## Known Issues
* classes for 1975 data mostly missing (~72,000) 
* titles truncated beyond 256 characters -- needs schema adjustment 
* locations in `location_inventor` table are listed from oldest to most-recent for an inventor career. Should make the  switch
  to most-recent only. Use `pd.drop_duplicates(take_last=True)` or some similar
  API call
* locations in `location_assignee` table have duplicates, also listeed from  oldest to most-recent for an assignee portfolio. Should make the switch to
  most-recent only.

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
