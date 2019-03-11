# TIPS

## CREATE MODEL
For this, necessary create a model with command:
````sh
rails generate model @model_name @param1:@type @param2:@type
````

Ex:
````sh
rails generate model task description:string status:boolean
````

Will be create a **tasks** model with params [**description**, **status**]

## 

## UPDATE MODEL

### ADDING COLUMNS
For this, necessary update a model with command:
````sh
rails generate migration Add@migrationNameTo@modelName @param1:@type @param2:@type
````

Ex:
````sh
rails generate migration AddSomeColumnsToTasks elapsed_time:integer difficulty:integer
````

Will be update a **tasks** model, adding params [**elapsed_time**, **difficulty**]

### REMOVING COLUMNS
For this, necessary update a model with command:
````sh
rails generate migration Remove@migrationNameFrom@modelName @param1:@type @param2:@type
````

Ex:
````sh
rails generate migration RemoveSomeColumnsFromRecipe elapsed_time:integer difficulty:integer
````

Will be update a **tasks** model, removing params [**elapsed_time**, **difficulty**]

## 

## TESTING
Having a service simply run the command:
````sh
rails db:migrate
````
This command will be create or update your tables

## 


To persist data will be create many itens on **Model**.
_You can use_
````sh 
rails console
````

````rails
@Model.create(@param1: @value1, @param2: @value2, @param3: @value3, @param4: @value4)
````

Ex:
````rails
Task.create(description: 'Buy a item', status: false, elapsed_time: 10, difficulty: 3)
````
