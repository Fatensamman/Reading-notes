## SQL
- Structured query language (SQL): a language designed for the query, manipulation and translation of data from a relational database for technically and non-technical users. And since it is easy, SQL databases provide secure and scalable storage for millions of websites and smartphone apps.
### examples:
```
ar mysql = require('mysql');

var con = mysql.createConnection({
  host: "localhost",
  user: "yourusername",
  password: "yourpassword"
});

con.connect(function(err) {
  if (err) throw err;
  console.log("Connected!");
});
```