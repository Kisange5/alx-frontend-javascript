0x02. ES6 classes
Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

How to define a Class
How to add methods to a class
Why and how to add a static method to a class
How to extend a class from another
Metaprogramming and symbols
Requirements
All your files will be executed on Ubuntu 18.04 LTS using NodeJS 12.11.x
Allowed editors: vi, vim, emacs, Visual Studio Code
All your files should end with a new line
A README.md file, at the root of the folder of the project, is mandatory
Your code should use the js extension
Your code will be tested using Jest and the command npm run test
Your code will be verified against lint using ESLint
Your code needs to pass all the tests and lint. You can verify the entire project running npm run full-test
Setup
Install NodeJS 12.11.x
(in your home directory):

curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh
sudo bash nodesource_setup.sh
sudo apt install nodejs -y
$ nodejs -v
v12.11.1
$ npm -v
6.11.3
Install Jest, Babel, and ESLint
in your project directory, install Jest, Babel and ESList by using the supplied package.json and run npm install.

Configuration files
Add the following files to your project directory.

package.json
Click to show/hide file contents
babel.config.js
Click to show/hide file contents
.eslintrc.js
Click to show/hide file contents
and…
Don’t forget to run $ npm install when you have the package.json

Tasks
0. You used to attend a place like this at some point
mandatory
Implement a class named ClassRoom:

Prototype: export default class ClassRoom
It should accept one attribute named maxStudentsSize (Number) and assigned to _maxStudentsSize
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 0-classroom.js

1. Let's make some classrooms
Import the ClassRoom class from 0-classroom.js.

Implement a function named initializeRooms. It should return an array of 3 ClassRoom objects with the sizes 19, 20, and 34 (in this order).
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 1-make_classrooms.js

2. A Course, Getters, and Setters
Implement a class named HolbertonCourse:

Constructor attributes:
name (String)
length (Number)
students (array of Strings)
Make sure to verify the type of attributes during object creation
Each attribute must be stored in an “underscore” attribute version (ex: name is stored in _name)
Implement a getter and setter for each attribute.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 2-hbtn_course.js

3. Methods, static methods, computed methods names..... MONEY
Implement a class named Currency:

- Constructor attributes:
code (String)
name (String)
Each attribute must be stored in an “underscore” attribute version (ex: name is stored in _name)
Implement a getter and setter for each attribute.
Implement a method named displayFullCurrency that will return the attributes in the following format name (code).
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 3-currency.js

4. Pricing
Import the class Currency from 3-currency.js

Implement a class named Pricing:

Constructor attributes:
amount (Number)
currency (Currency)
Each attribute must be stored in an “underscore” attribute version (ex: name is stored in _name)
Implement a getter and setter for each attribute.
Implement a method named displayFullPrice that returns the attributes in the following format amount currency_name (currency_code).
Implement a static method named convertPrice. It should accept two arguments: amount (Number), conversionRate (Number). The function should return the amount multiplied by the conversion rate.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 4-pricing.js

5. A Building
Implement a class named Building:

Constructor attributes:
sqft (Number)
Each attribute must be stored in an “underscore” attribute version (ex: name is stored in _name)
Implement a getter for each attribute.
Consider this class as an abstract class. And make sure that any class that extends from it should implement a method named evacuationWarningMessage.
If a class that extends from it does not have a evacuationWarningMessage method, throw an error with the message Class extending Building must override evacuationWarningMessage
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 5-building.js

6. Inheritance
Import Building from 5-building.js.

Implement a class named SkyHighBuilding that extends from Building:

Constructor attributes:
sqft (Number) (must be assigned to the parent class Building)
floors (Number)
Each attribute must be stored in an “underscore” attribute version (ex: name is stored in _name)
Implement a getter for each attribute.
Override the method named evacuationWarningMessage and return the following string Evacuate slowly the NUMBER_OF_FLOORS floors.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 6-sky_high.js

7. Airport
Implement a class named Airport:

Constructor attributes:
name (String)
code (String)
Each attribute must be stored in an “underscore” attribute version (ex: name is stored in _name)
The default string description of the class should return the airport code (example below).
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 7-airport.js

8. Primitive - Holberton Class
Implement a class named HolbertonClass:

Constructor attributes:
size (Number)
location (String)
Each attribute must be stored in an “underscore” attribute version (ex: name is stored in _name)
When the class is cast into a Number, it should return the size.
When the class is cast into a String, it should return the location.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 8-hbtn_class.js

10. Vroom
Implement a class named Car:

Constructor attributes:
brand (String)
motor (String)
color (String)
Each attribute must be stored in an “underscore” attribute version (ex: name is stored in _name)
Add a method named cloneCar. This method should return a new object of the class.
Hint: Symbols in ES6
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 10-car.js

11. EVCar
Import Car from 10-car.js.

Implement a class named EVCar that extends the Car class:

Constructor attributes:
brand (String)
motor (String)
color (String)
range (String)
Each attribute must be stored in an “underscore” attribute version (ex: name is stored in _name)
For privacy reasons, when cloneCar is called on a EVCar object, the object returned should be an instance of Car instead of EVCar.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x02-ES6_classes
File: 100-evcar.js
