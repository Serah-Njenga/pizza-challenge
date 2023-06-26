Learning Goals
Implement a 'mini' Rails application that implements associations.
Introduction
For this assessment, you'll be working on an API for tracking pizzas restaurants.

The instructions below will walk you through the process of ideation and planning your app: deciding on your models and relationships, planning how the information will be laid out on the page, etc. You should work through all the planning steps before you start doing any coding.

Requirements
For this project, you must:

Create a Rails API backend.
Have at least three resources (three DB tables).
 

Project Setup
Once you have the plan in place for the application you want to build take the following steps:

Create a new Rails project.
Create a new GitHub repository (NB: ENSURE IT IS PRIVATE).
Add your TM as a contributor to the project. (This is only for grading purposes. We promise, we won't steal your code)
Ensure you regularly commit to the repository.
Project Guidelines
Your project should conform to the following set of guidelines:

 Models
You need to create the following relationships:

- A `Restaurant` has many `Pizza`s through `RestaurantPizza`
- A `Pizza` has many `Restaurant`s through `RestaurantPizza`
- A `RestaurantPizza` belongs to a `Restaurant` and belongs to a `Pizza`

Start by creating the models and migrations for the following database tables:

domain-1.png

Add any code needed in the model files to establish the relationships. Then, run the migrations.

 You are welcome to generate your own seed data to test the application.

Validations
Add validations to the `RestaurantPizza` model:

- must have a `price` between 1 and 30

Routes
Set up the following routes. Make sure to return JSON data in the format
specified along with the appropriate HTTP verb.
