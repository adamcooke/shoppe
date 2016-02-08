# Shoppe

Shoppe is an Rails-based e-commerce platform which allows you to easily introduce a
catalogue-based store into your Rails 4 applications.

***How is this different to [tryshoppe/shoppe](https://github.com/tryshoppe/shoppe)]?**
Unfortunately, due to some poor management of pull requests and contributions on
my part, the main version of Shoppe has become unmaintainable by me and I cannot
continue to support it. In light of this, I have decided to maintain my own version
of Shoppe based on my own last known "good" version. I can only apologise for my
poor management of the original version. Apologies.

In the meantime, why not:

* [Check out the website](http://tryshoppe.com)
* [View the demo site](http://demo.tryshoppe.com)
* [Check out the demo site source](http://github.com/tryshoppe/example-store)
* [Read the release notes](https://github.com/tryshoppe/core/blob/master/CHANGELOG.md)
* [Read API documentation](http://api.tryshoppe.com)

## Features

* An attractive & easy to use admin interface with integrated authentication
* Full product/catalogue management
* Stock control
* Tax management
* Flexible & customisable order flow
* Delivery/shipping control, management & weight-based calculation

## Getting Started

Shoppe provides the core framework for the store and you're responsible for creating
the storefront which your customers will use to purchase products. In addition to
creating the UI for the frontend, you are also responsible for integrating with whatever
payment gateway takes your fancy.

### Installing into a new Rails application

To get up and running with Shoppe in a new Rails application is simple. Just follow the
instructions below and you'll be up and running in minutes.

    rails new my_store
    cd my_store
    echo "gem 'shoppe'" >> Gemfile
    bundle
    rails generate shoppe:setup
    rails generate nifty:attachments:migration
    rails generate nifty:key_value_store:migration
    rake db:migrate shoppe:setup
    rails server

## License

Shoppe is licenced under the MIT license. Full details can be found in the MIT-LICENSE
file in the root of the repository.
