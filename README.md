# NPM Contribution Assignment
## This Project creates and publishes a JavaScript package to NPM that prints your name to the console when used.
To make this project work you should 1.Create a GitHub Repository and clone it 
2. Create an NPM Account 
3. Set Up Your Project Open your terminal, navigate to the cloned repository folder, and initialize your project by typing npm init -y. This will create a package.json file with default settings. 
4. Write Your JavaScript Code Create a file named index.js in the project folder. In index.js, write code using console.log to print your name.
5. Add a bin to your package.json file Edit the package.json file and add the following,
"bin": {

"your-name": "index.js"

},