## Technologies Used

This project utilizes the following technologies:

- **MongoDB**: A NoSQL database used for storing and retrieving data.
- **jQuery**: A JavaScript library that simplifies HTML document traversing, event handling, and AJAX interactions.
- **AJAX**: Asynchronous JavaScript and XML, used for making asynchronous requests to the server without reloading the page.

### MongoDB Connection Example
```javascript
const MongoClient = require('mongodb').MongoClient;
const url = 'mongodb://localhost:27017';
const dbName = 'mydatabase';

MongoClient.connect(url, { useNewUrlParser: true, useUnifiedTopology: true }, (err, client) => {
    if (err) throw err;
    console.log("Connected successfully to MongoDB");
    const db = client.db(dbName);
    client.close();
});

jQuery and AJAX Example

$(document).ready(function(){
    $.ajax({
        url: 'https://api.example.com/data',
        method: 'GET',
        success: function(data) {
            console.log(data);
        },
        error: function(error) {
            console.error("Error fetching data:", error);
        }
    });
});

git add README.md
git commit -m "Updated README to include MongoDB, jQuery, and AJAX"
git push origin main

