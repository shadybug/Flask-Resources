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

# Phase 1
- Add routes: “/login” route, “/signup” route, and “/logout” route
- Code the “signup” method to retrieve data from the form, check for errors, and save the username and password in the
database.
- Code the “login” method to login the user and set a session
- Code the “logout” method. End the session and logout.
- Modify the home route to check sessions and log in the user if they previously logged in.
- - Basically, if there is a session, render the home page, otherwise render the welcome page so they have to login or
signup.
- - When there is a session, make sure you render the homepage with:
- - - The user variable set to the session username, and
- - - Set the list variable to empty (list = ‘ ‘) because the home page checks the list variable to see if there are events
to display on the homepage. At this stage of the application development, the home page won’t be displaying
any events yet. That’s why the list variable you pass to the home page should be empty.
`render_template('home.html', user = session['username'], list=list)`
