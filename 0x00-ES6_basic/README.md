0x00. ES6 Basics
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
Add the files below to your project directory

package.json
Click to show/hide file contents
babel.config.js
Click to show/hide file contents
.eslintrc.js
Click to show/hide file contents
Finally…
Don’t forget to run npm install from the terminal of your project folder to install all necessary project dependencies.

Tasks
0. Const or let?
Modify

function taskFirst to instantiate variables using const
function taskNext to instantiate variables using let
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 0-constants.js

1. Block Scope
Given what you’ve read about var and hoisting, modify the variables inside the function taskBlock so that the variables aren’t overwritten inside the conditional block.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 1-block-scoped.js

2. Arrow functions
Rewrite the following standard function to use ES6’s arrow syntax of the function add (it will be an anonymous function after)
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 2-arrow.js

3. Parameter defaults
Condense the internals of the following function to 1 line - without changing the name of each function/variable.

Hint: The key here to define default parameter values for the function parameters.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 3-default-parameter.js

4. Rest parameter syntax for functions
Modify the following function to return the number of arguments passed to it using the rest parameter syntax
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 4-rest-parameter.js

5. The wonders of spread syntax
Using spread syntax, concatenate 2 arrays and each character of a string by modifying the function below. Your function body should be one line long.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 5-spread-operator.js

6. Take advantage of template literals
Rewrite the return statement to use a template literal so you can the substitute the variables you’ve defined.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 6-string-interpolation.js

7. Object property value shorthand syntax
Notice how the keys and the variable names are the same?

Modify the following function’s budget object to simply use the keyname instead.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 7-getBudgetObject.js

8. No need to create empty objects before adding in properties
Rewrite the getBudgetForCurrentYear function to use ES6 computed property names on the budget object
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 8-getBudgetCurrentYear.js

9. ES6 method properties
Rewrite getFullBudgetObject to use ES6 method properties in the fullBudget object
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 9-getFullBudget.js

10. For...of Loops
Rewrite the function appendToEachArrayValue to use ES6’s for...of operator. And don’t forget that var is not ES6-friendly.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 10-loops.js

11. Iterator
Write a function named createEmployeesObject that will receive two arguments:

departmentName (String)
employees (Array of Strings)
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 11-createEmployeesObject.js

12. Let's create a report object
Write a function named createReportObject whose parameter, employeesList, is the return value of the previous function createEmployeesObject.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 12-createReportObject.js

13. Iterating through report objects
Write a function named createIteratorObject, that will take into argument a report Object created with the previous function createReportObject.

This function will return an iterator to go through every employee in every department.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 100-createIteratorObject.js

14. Iterate through object
Finally, write a function named iterateThroughObject. The function’s parameter reportWithIterator is the return value from createIteratorObject.
Repo:

GitHub repository: alx-frontend-javascript
Directory: 0x00-ES6_basic
File: 101-iterateThroughObject.js
