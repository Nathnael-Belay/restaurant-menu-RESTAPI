This project is a RESTful API which handles logs of food items on a restaurant menu.

I used LoopBack to make the API. LoopBack is a highly extensible, open source Node.js framework used
to create dynamic, end-to-end REST APIs very rapidly. APIs generated via LoopBack are Swagger APIs.

To run the project you'll have to make sure Node.js, loopback and MongoDB are installed. And MongoDB server running.
To instaall loopback
>npm install -g loopback-cli
To install the mongodb connector
>npm install --save loopback-connector-mongodb

Run the application
>node .

Then open the link http://localhost:3000/explorer to view the API

There are two models; dishes and User. 

--> Create a user using the POST/Users. Example:
	{
 	 "username": "Example",
 	 "email": "example@gmail.com",
 	 "password": "example"
	}
--> Click the try it out button. The response code will be 200 if successful, if not make sure you've entered the user using the proper syntax.
same goes for dishes, but it only has two propeties, name and price.

--> All dishes can be viewed using the GET/dishes route
--> PUT/dishes/{id} to edit a dish
--> DELETE/dishes/{id} to delete

Same goes for users.


