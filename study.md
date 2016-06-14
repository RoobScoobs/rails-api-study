# Rails as an API Study

Use your favorite search engine and the provided readings to research and answer
the following questions (no prior knowledge is expected).

In your answers, be sure to cite any relevant sources you consulted in your
search. We ask you to write answers in your own words in order to see how you
process what you've read. Please do not answer with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [rails-api-template](/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   [Starting Ruby on Rails: What I Wish I Knew | BetterExplained](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
-   [Intermediate Rails: Understanding Models, Views and Controllers | BetterExplained](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)
-   [The Rails Command Line — Ruby on Rails Guides](http://guides.rubyonrails.org/command_line.html)
-   [Rails Routing from the Outside In — Ruby on Rails Guides](http://guides.rubyonrails.org/routing.html)
-   [Action Controller Overview — Ruby on Rails Guides](http://guides.rubyonrails.org/action_controller_overview.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
In rails models are defined as Ruby classes that enable you to communicate with the
database. In addition to talking to the database, models store and validate data.
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
In the MVC architecture, it seems like controllers play the role of the boss while
acting as the middleman between the model and view. They simply receive specific
requests for the application and pass those requests to the model and view. They
are responsible for parsing user requests, data submissions, and sessions.
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
The purpose of routing is to decide which controller receives which requests. In other words,
the router takes in the URLs and sends them to a controller's action. Besides directing it
to a particular controller, the router also generates paths and URLS.   
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
A GET request to a URL address means that it wants to perform a specific operation
on a resource. The rails router then determines which controller and action to use for the request
(in this case it is fetching data). The controller receives the request, an instance
of that controller is created from the model, the method that exists within that class runs,
and a view is used to output the HTML.  
```
