# express_lab
Learning Objectives
Practice setting up express applications.
Practice creating custom routes.
Practice using parameters from a request.
Setup
Initialize your node modules by running npm init. Create a server file named server.js. Be sure you set the entry point property in package.json to the name of your server file.

Install express npm install --save express. Check your files. Hint: You can check to make sure your installation was successful in one of the following places:

Your package.json file should have express listed in the dependencies.
You could also check in your node_modules folder to see anexpress folder.
🐘 Need a reminder about getting and sending info?

app.get('/greeting/:name', (req, res) => {
  res.send({params: req.params, queries: req.query})
});
Meet These Specifications
Greetings
Your app should have a route of '/greeting/' and it should send a generic greeting to the screen like "Hello, stranger".

Your app should have a route of '/greeting/:name' and it should expect 1 param which takes in a person's name. When hitting the route, the page should display a message such as "Hello, ", or "What's up, <name>", or "<name>! It's so great to see you!" (ex. hitting '/greeting/Jimmy-boy' should display Wow! Hello there, Jimmy-boy on the page).

🔴 Commit 1 

"Commit 1: Greeting express application created."
Tip Calculator
Your app should have a route of '/tip' and it should expect 2 params. One should be total and one should be tipPercentage.

When hitting the route, the page should display how much your tip will be based on the total amount of the bill and the tip percentage. (ex. hitting '/tip/100/20' should display 20 on the page).

🔴 Commit 2 

"Commit 2: Tip Calculator express application created."
Magic 8 Ball
Create a route of '/magic' that should expect a phrase in the URL that ask the Magic 8 ball a question.

So if the user hits that route and asks a question of "Will I be a Millionaire" (ex. '/magic/Will%20I%20Be%20A%20Millionaire') they should see returned to them their question AND a random Magic 8 ball response (see the array below) on the screen.

Remember that we can't use spaces in the url, so we use %20 to express a space in the url.

Use this array of Magic 8 ball responses.....
["It is certain", "It is decidedly so", "Without a doubt", "Yes definitely","You may rely on it", "As I see it yes", "Most likely", "Outlook good","Yes", "Signs point to yes", "Reply hazy try again", "Ask again later","Better not tell you now", "Cannot predict now", "Concentrate and ask again","Don't count on it", "My reply is no", "My sources say no","Outlook not so good", "Very doubtful"]
🔴 Commit 3 

"Commit 3: Magic 8 Ball express application created."
Intro to the Internet
Read these notes

Watch this video about the internet AND this video about packets travel on the internet.

Optional: Hungry for more?
Fibonacci
Create a route 'fibonacci'

This route will take one param, the number we will operate on.

If the number param is not a fibonacci number, print out "I can tell this ain't a fibonacci number. Wack."

If the number is a Fibonacci number print out "Sweet Fibonacci number!."

🔴 Commit 4 

"Commit 4: Fibonacci application created."
Fibonacci Continued
Instead, take in a number that will refer to the index of a Fibonacci number. Print out the Fibonacci number that is located at that index.
Example:
The Fibonacci sequence:
1,1,2,3,5,8,13,21,34,55,89,144, ...;

num = 4

Output => 5
🔴 Commit 5 

"Commit 5: Hungry for more: Fibonacci application extended."
