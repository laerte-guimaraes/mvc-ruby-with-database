# TIPS

For this, necessary create a model with command:
````sh
rails generate model @model_name @param1:@type @param2:@type
````

Ex:
````sh
rails generate model task description:string status:boolean
````

Will be create a **taks** model with params [**description**, **status**]

## 

Having a service simply run the command:
````sh
rails db:migrate
````
This command will be create tables

## 

To persist data will be create many itens on **Model**.
_You can use_
````sh 
rails console
````

````rails
@Model.create(@param1: @value1, @param2: @value2)
````

Ex:
````rails
Task.create(description: 'Buy a item', status: false)
````