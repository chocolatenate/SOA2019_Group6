# How to run Service
## Request Service
### Change Directory
use command `cd request`

### Set Up MongoDB
1. make sure your computer be installed mongoDB and MongoShell started already.
2. import mockup database use this command.
 
 `mongoimport --db notification --collection mechanics --file mechanics.json`
 
### Install node module
use command. `npm install`

### Start server to run a service
use command. `npm start`

### Request Endpoint

| Event                     | Description                                   | 
|---------------------------|---------------------------------------------|
| `/api/request:id` |  update status to request mechanic to fix with mechnicId | 
### Test Endpoint
1. make sure your computer be installed mongoDB and MongoShell started already.
2. run test by this command `npm test`


## Other Service
### Set Up MongoDB
1. make sure your computer be installed mongoDB and MongoShell started already.
 2. import mockup database use this command.
 
 `mongoimport --db payang --collection mechanics --file mechanics.json`
 
 `mongoimport --db payang --collection customers --file customers.json`

### Install node module
use command. `npm install`

### Start server to run a service
use command. `npm start`

# Mechanic Endpoint

| Event                     | Description                                   | 
|---------------------------|---------------------------------------------|
| `/api/mechanics/find` | get information of all mechanics. | 
| `/api/mechanics/find/:id` | get information of mechanic by ID. | 
| `/api/mechanics/find/garage/:shopname` | get information of mechanic by Garage name ( shop name ). | 
| `/api/mechanics/updatestatus/:id` | update status of mechanic by ID. | 
| `/api/mechanics/updatecounter/:id` | increate a number of customer of mechanic by ID.|
| `/api/mechanics/register` | register new mechanic by request body.|

# Login Endpoint

| Event                     | Description                                   | 
|---------------------------|---------------------------------------------|
| `/api/login` |  post request body to compile with hash password for login. | 

# Customer Endpoint

| Event                     | Description                                   | 
|---------------------------|---------------------------------------------|
| `/api/customers/:id` |  get information of customer by ID.|
| `/api/customers/register` |  post request body to save in Database.| 

# Test Endpoint
1. make sure your computer be installed mongoDB and MongoShell started already.
2. cd to directory 'api'
3. run test by this command `npm test`
