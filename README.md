Hello All!

The purpose of this Laravel Demo Project is to demonstrate my skills of using various intermediate and advanced concepts of the framework. 
I am using Laravel version 7.4.0

More info about me:
My website: https://www.olivervoros.com 
LinkedIN: https://www.linkedin.com/in/olivervoros

Initial Project Setup:

run composer install
run npm install
CREATE DATABASE {database_name}
Edit your .env file to have a database connection using the newly created DB

And now let's see the examples:

1, Facades -> git checkout facades

Facade is an OOP design pattern, it is an object that serves as a front-facing interface masking more complex underlying or structural code. Facades are an important concept of Laravel. 
I have developed a WeatherForecast Facade, which demonstrated how Facades work in Laravel.

2, Eloquent Relationships -> git checkout eloquent-relationships

This branch demonstrates all the possible Eloquent relationships.

You will need the following steps to set up the database:

    1, php artisan migrate
    2, php artisan db:seed

You can see all the modeled relationships used in the AirlineController.

3, Service Container and Route-Model-Binding -> git checkout service-container

This branch shows the way to add a service to the container, and also various ways of route model bindings.

    1, php artisan migrate
    2, php artisan db:seed

4, Collections git checkout collections

There are tons of functions/methods you can use on "Laravel collections". I will examine and try a bulk of these functions...
