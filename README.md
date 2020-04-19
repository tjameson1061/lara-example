#Hello All!

![Alt Text](https://media.giphy.com/media/pxwlYSM8PfY5y/giphy.gif)

I have created this Github Account to demonstrate my skills of using various intermediate and advanced concepts of the Laravel framework.
My Setup: 
PHP 7.4.2, Laravel version 7.4.0, Composer, MySQL, Ubuntu, Apache

You can read more about me:   
My website: https://www.olivervoros.com    
My LinkedIN profile: https://www.linkedin.com/in/olivervoros   

Initial Project Setup:
Run composer install  
Run npm install  
CREATE DATABASE {database_name}  
Edit your .env file to have a database connection using the newly created DB  

Then select the required branch and issue git checkout {branch}   
After you checked out the branch, run composer dump-autoload   
Then php artisan migrate::refresh --seed   
Run the server by adding php artisan serve   

<u><b>And now let's see the examples:</b></u>   

1, <a href="#sc">Service Container</a>  
2, <a href="#fac">Facades</a>  
3, <a href="#eloq-rel">Eloquent Relationships</a>  
4, <a href="#coll">Collections</a>  
5, <a href="#wc">View Composers</a>  
6, <a href="#repo">Using the Repository Pattern</a>  
7, <a href="#mw">Middlewares</a>  
8, <a href="#sd">Soft Delete</a>  
9, <a href="#aam">Accessors and Mutators</a>  
10, <a href="#pipe">Pipelines</a>  
11, <a href="#noty">Notifications</a>  
12, <a href="#macros">Macros</a>  
13, <a href="#eaq">Events and Queues</a>  
14, <a href="#lat">Localization and Translation</a>  
15, <a href="#lel">Lazy or Eager Loading and the N+1 problem</a>  

1, <a name="sc">Service Container and Route-Model-Binding</a> -> git checkout service-container         
This branch shows the way to add a service to the container, and also various ways of route model bindings.

2, <a name="fac">Facades </a> -> git checkout facades    
Facade is an OOP design pattern, it is an object that serves as a front-facing interface masking more complex underlying or structural code. Facades are an important concept of Laravel. 
I have developed a WeatherForecast Facade, which demonstrated how Facades work in Laravel.

3, <a name="eloq-rel">Eloquent Relationships</a> -> git checkout eloquent-relationships       
This branch demonstrates nine possible Eloquent relationships.
The modeled relationships can be found in the AirlineController.

4, <a name="coll">Collections git checkout collections</a> -> git checkout collections       
There are loads of methods you can use on "Laravel collections". I try a number of these methods to learn their use case.

5, <a name="wc">View Composers</a> -> git checkout view-composers     
View Composers are a great way to share data between various views.
Implementation: see AppServiceProvider boot() method

6, <a name="repo">Repository Pattern</a>

7, <a name="mw">Middlewares</a>

8, <a name="sd">Soft Delete</a>

9, <a name="aam">Accessors and Mutators</a>

10, <a name="pipe">Pipelines</a>

11, <a name="noty">Notifications</a>

12, <a name="macros">Macros</a>

13, <a name="eaq">Events and Queues</a>    
A simple example of Events, Listeners and Queues.   
The implementation: Within the RegisterController we register a user, and if the user wins we trigger 
the RegisteredUserWonEvent. In the EventServiceProvider class we add two listeners to the RegisteredUserWonEvent.
Both listener's handle method is triggered, and as the listener classes implement ShouldQueue, 
the listener tasks are added to the database driven queue. (see: .ENV QUEUE_CONNECTION=database) 

14, <a name="lat">Localization and Translation</a>     
A simple implementation of using multiple languages within a Laravel application.
For the implementation check: the lang directory and the welcome.blade.php view file.

15, <a name="lel">Lazy or Eager Loading and the N+1 Problem</a>     
This branch explains the N+1 problem, and shows a way to optimise the given database queries.
I suggest, that you set up telescope in order to see the list of SQL queries.
More here: https://laravel.com/docs/7.x/telescope
For the implementation check: ArticleController
