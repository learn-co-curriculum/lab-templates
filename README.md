# Lab Outline:

Labs should always have **specs** that involves writing code to pass tests

##Examples

## Format of a Lab Readme
### `#` Title
The title comes first. It should be the name of the repository.

### `##` Objectives
Objectives Should immediately follow the title of the lab. Students should be able to readily find and define the skills they should be expected to practice or learn by completing the lab.

### `##` Introduction

The introduction should discuss the premise, or scenario of the lab. It should set the stage for the work the students will be doing. You don't need to title it as "Introduction." Feel free to be creative. 

### `##` Instructions

Instructions should be a numbered list of steps to take when solving the lab. This section can include a leading paragraph if its content does not fit into the numerical order (i.e. "After forking and cloning this lab, open the `*.xcworkspace` file.").

## Lab Templates

* fundamental-ruby
* command-line
* SQL
* activerecord
* rake
* erb-static-site
* rack
* sinatra-classic
* sinatra-mvc
* js
* front-end

Note for rails labs moving forward we should be using [flatiron-rails](https://github.com/flatiron-school/flatiron-rails) to generate new Rails labs.

###Fundamental Ruby
  File Structure:
  ```bash
  ├── README.md             # The guide to the this lab
  ├── Gemfile               # A file that specifies helpful external Ruby libraries
  ├── Gemfile.lock          # A file created by bundler that stores the specific versions of gems
  ├── lib/                  # The directory that holds your programs code
  │   └── file.rb           # The Ruby file where your code goes
  └── spec/                 # The directory where test files go
      └── spec_helper.rb    # This rspec file instructs all test files how
      └── file_spec.rb      # The test itself, which is testing only file.rb
  ```

###Command Line
  File Structure:
  ```bash
  ├── README.md
  ├── Gemfile
  ├── bin/                  # The directory that holds code only meant to execute the program
  │   └── runner.rb         # The file that executes the program
  ├── lib/
  │   ├── environment.rb    # The file that requires all the different parts of your program
  │   └── lab-name/         # The directory that holds the core of your program
  │       └── cli.rb        # The main file of your program
  └── spec/
      └── spec_helper.rb
      └── file_spec.rb
  ```

###SQL
  File Structure:
  ```bash
  ├── README.md
  ├── Gemfile
  ├── bin/
  │   ├── environment.rb
  │   ├── run.rb            # The same as runner.rb
  │   └── sql_runner.rb     # The file that instructs ruby how to evaluate your SQL
  ├── lib/
  │   └── sample.sql        # The file that your SQL goes in
  └── spec/
      └── spec_helper.rb
      └── file_spec.rb
  ```

###ActiveRecord
  File Structure:
  ```bash
  ├── README.md
  ├── Gemfile
  ├── Rakefile              # Holds ruby code that can be executed via the command line
  ├── app/                  # This directory organizes your application's components
  │   └── models/           # The directorty that the models go in
  │       └── sample-class.rb  # A model, which holds logic to interact with your database
  ├── config/               # This directory contains code to help run your app
  │   └── environment.rb
  ├── db/                   # This directory holds all your files that are relevant to your database
  │   └── migrations/       # This directory holds files that instruct your database about how to construct it's schema
  ├── lib/
  │   └── support/          # A directory that holds files help your program run
  │       ├── connection_adapter.rb  # This file specifies how to connect to your database
  │       └── db_registry.rb  # A file that instructs the connection_adapter to choose between a test, development, or production environment
  └── spec/
      └── spec_helper.rb
      └── file_spec.rb
  ```

###Rake
  File Structure:
  ```bash
  ├── README.md
  ├── Gemfile
  ├── Rakefile
  ├── bin/
  │   └── console   # Allows you enter a pry session with your entire app loaded into it
  ├── config/
  │   └── environment.rb
  ├── lib/
  │   └── file.rb
  └── spec/
      ├── rakefile_spec.rb
      └── spec_helper.rb
  ```

###Rack
  File Structure:
  ```bash
  ├── README.md
  ├── Gemfile
  ├── app/
  │   ├── application.rb
  │   └── controllers/      # A directory that holds controllers
  │       └── erb_maker.rb  # A file that helps interact between models and views
  ├── config/
  │   └── environment.rb
  ├── config.ru             # A file that executes rack files
  ├── lib/
  │   └── templates/        # A directory that holds files to be executed by
  │       └── my_cool_response.html.erb
  └── spec/
      ├── controllers/
      │   └── 01_server_port_spec.rb
      ├── spec_helper.rb
      └── support/
          └── an_ok_request.rb
  ```

###Sinatra Classic
  File Structure:
  ```bash
  ├── README.md
  ├── Gemfile
  ├── Rakefile
  ├── app.rb
  ├── config
  │   └── environment.rb
  ├── config.ru
  ├── models
  ├── public
  │   ├── images
  │   ├── javascripts
  │   └── stylesheets
  ├── spec
  │   └── spec_helper.rb
  └── views
  ```

###Sinatra MVC
  File Structure:
  ```bash
  ├── README.md
  ├── Gemfile
  ├── Rakefile
  ├── app
  │   ├── controllers
  │   │   └── application_controller.rb
  │   ├── models
  │   └── views
  │       └── layout.erb
  ├── config
  │   └── environment.rb
  ├── config.ru
  ├── db
  │   ├── migrate
  │   └── seeds.rb
  ├── public
  │   └── stylesheets
  └── spec
      ├── controllers
      ├── features
      ├── models
      └── spec_helper.rb
  ```

###Javascript
  File Structure:
  ```bash
  ├── README.md
  ├── css
  ├── images
  ├── index.html
  ├── js
  │   ├── file.js
  │   └── jquery-1.8.3.min.js
  ├── requires.yml
  └── spec
  ```

###Front-end
  File Structure:
  ```bash
  ├── README.md
  ├── css
  │   └── style.css
  ├── images
  └── index.html
  ```


<p data-visibility='hidden'>View <a href='https://learn.co/lessons/lab-templates' title='Lab Outline:'>Lab Outline:</a> on Learn.co and start learning to code for free.</p>
