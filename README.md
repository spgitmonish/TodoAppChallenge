Todo Application Coding Challenge
=======

This is a sample Todo application built as a coding challenge for potential candidates of CenturyLink CLARC.
Our desire is to provide a basic application that should be easy to get up and running, but that provides an
example toolset of a modern webstack.

Because of that desire, we have built this on the following projects or tools:
* TodoMVC (http://todomvc.com/examples/angularjs/#/)
* AngularJS v1 (https://angularjs.org/)
* Flask Micro Web Framework (http://flask.pocoo.org/)
* Sqlite Database (https://www.sqlite.org/)
* SQLAlchemy Python ORM (http://www.sqlalchemy.org/)

## The Assignment

You will be given a feature to be added to this application.  If you are familiar with Angular and Flask
(or similar micro frameworks) this assignment should take less than an hour.  If you are not familiar with
any of the tools, it will take a bit longer.

The assignment you are given will require you to add features to both the front-end (Angular, both js and html)
and the back-end (Flask).

Our suggestion is to get this application up and running and spend a couple hours working on the assignment.
If you are stuck after that time, message your contact and let us know where you at.  While we like finished
products, our desire is not for you to spend a ton of time on this assignment.

## Requirements

This application will run on Windows, Linux or OS X.  However it will take a little extra work to get things going
in Windows, and so if you choose to use it plan on spending a little more time getting things to work (one hint:
make sure Sqlite is running).

* Sqlite
* Python 3

## Quick Start
```
  git clone https://github.com/Cognilytics/todoChallenge.git
  cd todoChallenge
  <create and use virtualenv if desired>
  pip install -r requirements.txt
  python server.py
```
Open browser to http://localhost:3000

## Structure

A few important files to know about:

```
├── api.py							< Flask Restful Api File >
├── bower.json						< Bower File >
├── config.py						< Flask configuration file >
├── models.py						< SQLAlchemy Models >
├── requirements.txt				< Python Requirements File >
├── static							< Static Folder >
│   ├── lib								< Bower Libraries >
│   ├── scripts							< Angular Stuff >
│   │   ├── app.js
│   │   ├── controllers						< Angular Controllers >
│   │   │   └── todoCtrl.js
│   │   ├── directives						< Angular Directives >
│   │   │   ├── todoFocus.js					< Directive for focus >
│   │   │   └── todoEscape.js					< Directive for escape >
│   │   └── services                        < Angular Service for Communication >
│   │       └── todoStorage.js
│   └── styles							< CSS Stuff >
│       └── main.css
├── templates							< Flask Rendered Templates >
│   └── index.html						
├── test.db							< SQLite Database >
└── server.py						< Flask Main File >
```
