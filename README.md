
## Development 
### NodeJS Setup 


```
nvm install 14.17.1
```

### Setting up Express Library 
Library for creating app servers using nodejs. 

#### Installing Express

```bash
npm install express
```

```javascript

// server.js
const express = require('express')

const app = express()
app.get('/', (req, res) 
app.listen(4445, () => {
    console.log('Server started on http://localhost:4445')
})
```

### Database Setup 

Enter PSQL for Postgres 

```
# Linux 
sudo -u postgres psql 

# Mac 
psql postgres 
```

Create Database, User and Grant Privilege

Postgres   
```psql
create database sclrac;
create user sclrac with encrypted password 'sclrac';
grant all privileges on sclrac.* to sclrac;
```

MySQL   
```mysql
create database sclrac;
create user sclrac identified by 'sclrac';
grant all privileges on sclrac.* to sclrac;
```
