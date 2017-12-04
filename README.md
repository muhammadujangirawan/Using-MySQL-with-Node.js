# Using-MySQL-with-Node.js and Express Framework
This source code is an example of using MySQL for Node.js.

##Running Application
This source code is an example of using MySQL for Node.js.

Running Application
Run npm start command on the Node.js command prompt then see the logs that appear on the command prompt Node.js. 
If successful connect it will display Connection established if failed connect will display Error connecting to Db

Sample Connection

// connection to MySQL Database
const con = mysql.createConnection({
  host: 'localhost',
  user: 'root',
  password: '',
  database: 'nodejs'
});

con.connect((err) => {
  if(err){
    console.log('Error connecting to Db');
    return;
  }
  console.log('Connection established');
});
