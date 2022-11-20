# Phase 1

- Modify app.py to import the common flask libraries (request, redirect, session, render_template)
- Add database connection codes and config.py file
- Add codes to create a “users” table if it doesn’t exist already.
- - The table should have a primary key (id column), and at least 2 other columns: username, password (all these columns
can be VARCHAR type)
- Add codes to create an “events” table if it doesn’t exist already.
- - The table should have a primary key (id column), and at least 5 other columns: host, description, day, time, status (all
these columns can be VARCHAR type)
- Add a home route to render the welcome page (index.html file)
