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

# To add ESLINT you should

1. Verify Your Project Setup

Open your project in Visual Studio Code.
Ensure that your project directory contains a valid package.json file.
Ensure you can open an integrated terminal running a bash/zsh shell in the root folder.

2. Install ESLint

Install ESLint as a development dependency using npm.
npm install eslint --save-dev
After running this command, ESLint will be listed under devDependencies in your package.json file, and you can configure it according to your project’s requirements.

3. Run ESLint Initialization

In the integrated terminal, run the ESLint initialization command.
npm init @eslint/config
Follow the interactive prompts to answer configuration questions tailored to your project.

How would you like to use ESLint? To check syntax and find problems
What type of modules does your project use? None of these
Which framework does your project use? None of these
Does your project use TypeScript? No
Where does your code run? Node
... Would you like to install them (eslint, globals, @eslint/js) now? Yes
Which package manager do you want to use? npm
ESLint finishes resulting in an eslint.config.mjs file.
If needed, you can run this init script again if you need to change any answer.

4. Configure the Generated File

Open the generated eslint.config.mjs file in Visual Studio Code.
Review the default settings and adjust them as necessary to match your project’s coding style and requirements.
Ensure that the configuration includes all desired rules and plugins relevant to your project. Compare yourd with the eslint.config.mjs in this gist: ESLint Allow ConsoleLinks to an external site. 

5. Add a Lint Script to package.json
Open your package.json file in Visual Studio Code.

 Add a script entry that allows you to run ESLint on your code.
Ensure the commas is configured correctly to target the files you wish to lint.
"scripts": {
    "test": "echo \"error: no test specified\" && exit 1",
    "lint": "eslint index.js"
},
6. Run the Linting Process

Use the integrated terminal to execute the lint script you added.
Run the command:
npm run lint 

7. Fix Reported Issues

Address each linting error or warning by updating your code accordingly.
Continue running the lint command until your code passes all linting checks.
Repeat this as needed when you add more code to this project.
