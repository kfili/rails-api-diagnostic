# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```bash
A back end processes requests from a User/client/front end. It stores data in a
database and has an application to process and manage interactions with the
database and front end.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
Model
```

Which layer in the MVC pattern communicates with the model?

```bash
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
They are becoming obsolete
```

What does C.R.U.D stand for?

```bash
Create, Read, Update, Delete
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```bash
show, index, create, update, destroy
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
-The server forwards the request to the router
-The router interprets the request and sends corresponding commands to the
  Controller, including the table 'people' and ID '1'
-The controller calls methods on the model to retrieve the appropriate data
-The Model produces the appropriate data via SQL commands
-The controller returns the data to the server
-The server sends the data to the client.
```

What is the command to generate a new rails-api app?

```bash
bundle install
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails server
(or rails server?)
```

What are the commands to drop, create and migrate a database from the command
line? (3 bullet points)

```bash
rake db:create
rake db:drop
rake db:migrate
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
rails generate model ad name:string description:text price:decimal seller_id:integer email:string img_url:string
```
