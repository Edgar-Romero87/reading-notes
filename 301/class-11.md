# EJS

[EJS Tutorial](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

[Resource Google Books API](https://developers.google.com/books/docs/v1/using#WorkingVolumes)

[EJS Docs](https://ejs.co)

[EJS Tutorial](https://scotch.io/tutorials/use-ejs-to-template-your-node-application)

[Source Code for EJS Tutorial](https://github.com/scotch-io/node-ejs)


- First step - npm init
- then npm install express, body parser, cors, ejs
- var express = require (‘express);
- var body parser = require(‘body parser’);
- var cors = require (‘cors’);
- var path = require(‘path’);
- var expressLayouts = require(‘express-ejs-layouts’);
- var app = express();
- app.use(bodyParser());
- app.use(cors());
- app.use(expressLayouts);
- app.set(‘views’, path.join__dirname, ‘views’));
- app.set(‘view engine’, ‘ejs’);
- app.get(‘/, function(request, response){ response.render(‘index’, { foo: ‘bar’ }); takes the name of the file, not the filepath. – get route for the root directory.This is now making a variable call foo, that makes it available to use. })
- then set up a new folder called views, set up a file called index.ejs.
- app.listen(8000, function() { console.log(‘heard on 8000); })
- response. render takes in three parameters.
- this is helpful if you either have an API call or a delete call.
- you can also use this to manipulate arrays as well.
- this is super helpful if you have an < ul > that you need to manipulate.
- this gives us the ability to write an if/else statement as well, to make evaluations on the front end.
- layouts are not native to EJS. it is useful to have layout file and have everything wrapped in it.
- npm install –S express.ejs.layouts is the way to install it into your file.
