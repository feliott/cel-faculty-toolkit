# Community Engagement Toolkit website for CSC-324

Visit the current web app [here](https://cel-toolkit.herokuapp.com/).

## Introduction 

### Background and purpose:

This project is a website for the Community Engaged Learning toolkit for Grinnell faculty. Its purpose is to support faculty in community engaged courses and act as a central place for faculty to go to when they have questions. The client hopes for an interactive website that supports searching, exploring, and queries. The most important feature is searching (which has been implemented using Google search engine) that enables users to enter search terms and find related resources which can be in the form of different media types such as video, text, audio, etc...

### Structures

This project consists of glossary, search and many different static pages. In static pages, main contents are stored with a sidebar that allows users to jump to specific sections. Users can access glossary and search through the top navbar or homepage. Glossary provides users with a list of important terms for CEL, their explanations and associated sections that users can click. Search allows users to get related pages that contain the term they put in the search bar. The current search feature is programmed using Google search engine. No extra gem is used beside those used in standard rails application.

### Reference resources
○ 	[Ruby_on_Rails tutorial](http://www.railstutorial.org)

○ 	[Stack Overflow](https://stackoverflow.com/)

○ 	[Contentful with Rails](https://github.com/contentful/contentful_rails)

○ 	[Bootstrap 4 tutorial on W3school](https://www.w3schools.com/bootstrap4/)

○ 	[Programmable Search Engine](https://support.google.com/programmable-search)


## Getting started

To get started with the project, first clone the repo and `cd` into the directory:

```
$ git clone https://github.com/CSC322-Grinnell/324toolkit
$ cd toolkit_app
```

Then install the needed packages (while skipping any Ruby gems needed only in production):

```
$ yarn add jquery@3.5.1 bootstrap@3.4.1
$ bundle install --without production
```

If you run into any installation issues or missing dependencies, refer to this [first chapter](https://www.learnenough.com/ruby-on-rails-6th-edition-tutorial/beginning) of the Rails tutorial for details.

Next, migrate the database (for tag search):

```
$ rails db:migrate
```

Finally, run the test suite to verify that everything is working correctly:

```
$ rails test
```

If the test suite passes, you’ll be ready to seed the database with sample users and run the app in a local server:

```
$ rails db:seed
$ rails server
```
Now, visit http://localhost:3000/ in any browser in your local machine to see the running app

## Deploying

To deploy the sample app to production, you’ll need a Heroku account as instructed [Section 1.4, “Deploying”](https://www.railstutorial.org/book/beginning#sec-deploying) in the tutorial. Please contact the instructor for access and ownership of the current heroku account being used.

## Credit

This is made with the help of
[*Ruby on Rails Tutorial:
Learn Web Development with Rails*](https://www.railstutorial.org/)
(6th Edition)
by [Michael Hartl](http://www.michaelhartl.com/).
All content belongs to Grinnell College. 
