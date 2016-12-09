# facebook_watcher
Watch facebook comments and posts and answer from your neural network


![Facebook](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7c/Facebook_New_Logo_(2015).svg/1280px-Facebook_New_Logo_(2015).svg.png)

Install 
```javascript
npm install flyber_facebook_watcher
```

Use in your code
```javascript

var facebook_watcher = require("facebook_watcher");

var facebook_user = require("facebook_watcher/user");

var you = facebook_user({byLogin: "yourLogin", password: "password"});

var subscription = facebook_watcher.subscribe( {byFilter: "football"} );

subscription.on("post", function(post) {

    var text = post.text;
    
    //apply your code here
    
    you.reply(post, "your Comment");

});


subscription.on("comment", function(comment) {

    var text = comment.text;
    
    var postText = comment.post.text;
    
    //apply your code here
    
    you.reply(post, "your Comment For Post");
    
    you.reply(comment, "your Comment For Comment");

});



```

In order to get this working please contact to a.stegno@gmail.com

```Price
Subscription: 50$ per month. 
```

The website http://flyber.net

