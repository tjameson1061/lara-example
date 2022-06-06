
Tech Stack: 
PHP 7.4.2, Laravel, Composer, MySQL, Ubuntu, Apache, Vue JS

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
13, <a href="#eaq">Events, Listeners and Queues</a>  
14, <a href="#lat">Localization and Translation</a>  
15, <a href="#lel">Lazy or Eager Loading and the N+1 problem</a>  
16, <a href="#cbd">Custom Blade Directive</a>  
17, <a href="#siro">Signed Routes</a>  
18, <a href="#auth">Authorization</a>      
19, <a href="#bc">Broadcasting</a>  
20, <a href="#test">Unit Testing, Integration Testing, Browser Testing</a>      
21, <a href="#vue">Mini Project: Laravel API with VueJS</a>

1, <a name="sc"><b>Service Container and Route-Model-Binding</b></a>        
As the Laravel documentation says, the Laravel service container is a powerful tool for managing class dependencies and performing dependency injection.    
Dependency injection is a fancy phrase that essentially means this: class dependencies are "injected" into the class via the constructor or, in some cases, "setter" methods.   
This branch shows the way to add a service to the container, and also demonstrates various ways of route model bindings.
Implementation: https://github.com/olivervoros/laravel-demo-project/compare/service-container        

2, <a name="fac"><b>Facades</b></a>    
The Facade design pattern hides the complexities of the system and provides an interface to the client using which the client can access the system.    
I have developed a custom Facade called WeatherForecast, which demonstrates how Facades work in Laravel.
Implementation: https://github.com/olivervoros/laravel-demo-project/compare/facades       

3, <a name="eloq-rel"><b>Eloquent Relationships</b></a>   
This branch demonstrates nine possible Eloquent relationships.     

4, <a name="coll"><b>Collections</b></a>     
Collections in Laravel are wrappers around arrays of data, with numerous predefined methods, which helps you to work with the data.       
Under the "Collections branch", I try a number of these predefined methods to represent their use case.     

5, <a name="wc"><b>View Composers</b></a>     
View Composers are a great way to share data between various views.      

6, <a name="repo"><b>Repository Pattern</b></a>    
Repository pattern is a kind of container where data access logic is stored. 
It hides the details of data access logic from business logic. 
In other words, we allow business logic to access the data object without having knowledge of underlying data access architecture.     

7, <a name="mw"><b>Middlewares</b></a>      
By using middlewares you can modify or filter the incoming HTTP Request.    
In our implementation we apply an IP address checking middleware.     

8, <a name="sd"><b>Soft Delete</b></a>     
As the Laravel documentation says, when models are soft deleted, they are not actually removed from your database. 
Instead, a deleted_at attribute is set on the model and inserted into the database. 
If a model has a non-null deleted_at value, the model has been soft deleted.      

9, <a name="aam"><b>Accessors and Mutators</b></a>         
Accessors and mutators allow you to format Eloquent attribute values when you retrieve or set them on model instances.    

10, <a name="pipe"><b>Pipelines</b></a>            
Basically, using laravel pipelines you can pass an object between several classes in a fluid way 
to perform any type of task and finally return the resulting value once all the “tasks” have been executed.     

11, <a name="noty"><b>Notifications</b></a>         
Laravel provides support for sending notifications across a variety of delivery channels, including mail, SMS (via Nexmo), and Slack. 
Notifications may also be stored in a database, so they may be displayed in your web interface.     

12, <a name="macros"><b>Macros</b></a>      
Laravel Macro is a way to add some missing functionality to Laravel's internal component with a piece of code which doesn't exist in the Laravel class. 
To implement a Laravel Macro, Laravel provides a PHP trait called Macroable.     

13, <a name="eaq"><b>Events, Listeners and Queues</b></a>          
A simple example of Events, Listeners and Queues.   
The implementation: Within the RegisterController we register a user, and if the user wins we trigger 
the RegisteredUserWonEvent. In the EventServiceProvider class we add two listeners to the RegisteredUserWonEvent.
Both listener's handle method is triggered, and as the listener classes implement ShouldQueue, 
the listener tasks are added to the database driven queue. (see: .ENV QUEUE_CONNECTION=database)         

14, <a name="lat"><b>Localization and Translation</b></a>         
A simple implementation of using multiple languages within a Laravel application.
For the implementation check: the lang directory and the welcome.blade.php view file.      

15, <a name="lel"><b>Lazy or Eager Loading and the N+1 Problem</b></a>       
This branch explains the N+1 problem, and shows a way to optimise the given database queries.
I suggest, that you set up telescope in order to see the list of SQL queries.

16, <a name="cbd"><b>Custom Blade Directive</b></a>       
A very simple example of creating a custom blade directive...     

17, <a name="siro"><b>Signed Routes</b></a>       
A straightforward example of using signed routes. This is mostly used for account activations, or when you want to protect a route from users who do not know the URL signature.       

18, <a name="auth"><b>Authorization</b></a>         
Example code which includes various implementations of Laravel Authorization, such as Gates and Policies.      

19, <a name="bc"><b>Broadcasting</b></a>       
An example implementation of using Laravel's broadcasting feature.       

20, <a name="test"><b>Testing</b></a>                 
Few examples covering different software testing methods:      
- Unit Testing with Prophecy
- Unit Testing and Integration Testing
- Browser Testing with Dusk

21, <a name="vue"><b>Mini Project: Laravel API with VueJS</b></a>            
Laravel API with Passport Auth and HTTP testing on the backend and VueJS + Vuex on the frontend
# lara-example
