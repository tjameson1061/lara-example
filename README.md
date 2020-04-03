Hello All!

The purpose of this Laravel Demo Project is to demonstrate my skills of using various intermediate and advanced concepts of the framework. I am using Laravel version 6.

(My website: https://www.olivervoros.com for more info about me...)

And now let's see the examples:

1, Facades

Facade is an OOP design pattern, it is an object that serves as a front-facing interface masking more complex underlying or structural code. Facades are an important concept of Laravel. 
I have developed a WeatherForecast Facade, which demonstrated how Facades work in Laravel.
You can access the example by issuing "git checkout facades".

2, Eloquent Relationships

This branch demonstrates the various Eloquent relationships.

git checkout eloquent-relationships

You will need the following steps to set up the database:

1, Create a database
2, Edit your .env file to have a database connection using the newly created DB
3, Run the migration file: php artisan migration
4, Seed the Database in order to have some data: php artisan db:seed

Relationships modeled:
one-to-one -> Airline and Base
one-to-many -> Airline and Aircrafts
many-to-many -> Flight and Pilots
polymorphic-many-to-many Schedule, Pilots and Cabincrew