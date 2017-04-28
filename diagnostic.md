# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
Backends are servers. They receive http requests from clients and respond with the
appropriate data. They are also responsible for persisting the data.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
The controller tells the model to fetch data.
```

Which layer in the MVC pattern communicates with the model?

```md
The controller.
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Don't we? Model "View" Controller pattern.
```

What does C.R.U.D stand for?

```md
Create, read, update, destroy.
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
Model.
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
Create, user.new. Read, user.all, user.find_by. Update, user.update_all. Delete,
User.destroy.
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
1. Get request goes to the people controller (assuming the controllers are set
   up this way).
2. The people controller speaks to the people model and requests person with id one.
3. The people model retreives person one and gives it to the controller.
4. The people controller gives the data to the view.
5. The view displays the information to the user.
```

What is the command to generate a new rails-api app?

```bash
rails new api_name
```

What is the command to start an instance of a rails server?

```bash
bundle exec rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
rake db:drop db:create db:migrate db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate model PET [name :string, age :integer]
```
