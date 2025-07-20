Legend: 

\* : Explained later 

# General Concept

The project is about making a portfolio myself with full devops pipeline 

The goal is to host on there my real time project aswell as my web project and to train the devops methods as I work on it 

The design will be made mobile first 



# User Experience

## Home page 

On arrival the user will have a list of all my project ordered by most recent to least recent with a paging system

If the user want to target specific types of projects or used technology it can select differents types of filters* that will update in real time the projects available

If no project was made with the selected filters then a message is shown on screen 

The projects have a card* that is clickable


## Project Page 

This page has the main project's pictures as the banner then below it has the title of the project 

Then a general description of the projects

Then a general developpement description 

it will have the stack used 

then pictures of the project as a slider (if more than one picture)


## Project Cards 

* Main picture
* Prod Date
* Title
* Slider
  * Stack
  * Type



## Filters

* Language 
  * C++
  * C#
  * Python
  * Bash
  * Shell
  * etc.. 
* Frameworks/Library
* Type
  * Web
  * Real Time
* Versionning
  * Git
  * SVN 
* CI/CD
  * Github action
  * Jenkins 
* Conterization 
  * Docker


## Header

Mon logo (galaxy binaire)


## Footer 

Formulaire pour envoyer un mail si intéresser 


# Admin Controls 

Acessible via a route "/admin"

On arrival it ask a password  defined in .env file if correct it redirect us to the dashboard

## Dashboard 

A button to go to the User page 

## Header

A home logo to go to the user page 


## Projects 

A list of all current projects *

A button to add a project *


## Filters

#### Filter Tab

A list of all filters *

A button to add a filter *


#### Category Tab

A List of all categories *

A button to add a filter Category *

---


### List of projects

As a vertical list with a button to either edit or delete

On clicking edit it leads us to a edit page *

On clicking delete it shows us a warning message asking us to confirm if we are sure to delete the project 


* Title 
* Type
* Stacks

### List of filters 

As a vertical list 

A button to edit a filter 
* On clicking edit, the targeted filter inputs (name and category) becomes editable 
  * To change the name it's a basic text input 
  * To change the category it's a selector input
* A button "Save" saves changes to the database, a cancel button cancel all changes 

A button to delete a filter 
* Shows a popup confirming delete 

### List of categories

Same as list of filters but only the name is changeable (text input too)

### New Project 

A page with the necessary inputs to create a new project 

* Title (Text input)
* Project tyoe
* Stack used 
* Main picture (upload input )
* Main picture preview (not saved)
* Start time - End time (date time)
* Team (text input)
* Project description (text area) 
* development description (textarea)
* pictures of the project
* preview of the pictures 
* on the side locked pos
 * Sources

when canceling or saving changes it redirect us to the oroject page 

### Edit project 

Same as new but with info completed 


