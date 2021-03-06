# CS 262 Monopoly Webservice

This is the data service application for the [CS 262 sample Monopoly project](https://github.com/calvin-cs262-organization/monopoly-project)
and it is deployed here:

<https://cs262-monopoly-service.herokuapp.com/>

It is based on the standard Heroku with Node.js tutorial.

<https://devcenter.heroku.com/articles/getting-started-with-nodejs>

The database is relational with the schema specified in the `sql/` sub-directory,
 and is hosted on [ElephantSQL](https://www.elephantsql.com/). The database user
and password are stored as Heroku configuration variables rather than in this (public) repo.

We implement this sample as a separate repo to simplify Heroku integration, but
for lab 9, you can simply submit your code under the standard `cs262/lab09` directory.
For the team project, configure your Heroku app to auto-deploy the code from the
master/main branch of your
service repo; do this by following the instructions under the &ldquo;Deploy&rdquo;
tab in your application in the Heroku dashboard.

A. What are the (active) URLs for your data service?
Service URL Links:
* https://gentle-lowlands-28780.herokuapp.com/
* https://gentle-lowlands-28780.herokuapp.com/players
* https://gentle-lowlands-28780.herokuapp.com/players/1
* https://gentle-lowlands-28780.herokuapp.com/playersGame (2 joined tables)

B. Which of these endpoints implement actions that are idempotent? nullipotent?
* players and players/1 are nullipotent
* players is idempotent

C. Is the service RESTful? If not, why not? If so, what key features make it RESTful.
* The service is RESTful because it is stateless, supports JSON, and it is simple than SOAP.

D. Is there any evidence in your implementation of an impedance mismatch?
* There is no impedance mismatch.