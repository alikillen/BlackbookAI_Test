# BlackbookAI_Test

Repository to store my tech test for a junior position with Blackbook AI

Please see docs folder for test instructions PDF

From this PDF I have determined a series of steps:

Notes:

- most appropriate language is probably python (includes writing/reading data to CSV file, plus web scraping element)
- UIpath community edition account created - only works with windows
- Use UIpath for.....?

- create a react/js version first? jquery/npm modules allowed? then use python? upload python scripts into UIpath as robots?
- office excel CSV file created - see docs folder

- process needs to be automated and run a few times to populate data

# Steps:

## Use your workflow to populate Apple, Orange, Banana and one fruit of your choosing.

Create CSV file (can also be excel file)
look into UIpath and how to create automated workflow

1. Program takes user input, checks if it exists as a fruit in column A of CSV table
2. If it does not exist in CSV then:

   - search for the user's input in the USDA FoodData API
   - deserialise (string into object) the response
   - see if the word fruit exists in the response, then:

   3. if "Fruit" does not exist:

   - program tells user "I dont believe this is a fruit" and asks user to try again
   - user has 2 options: try again (returns to start input) and exit (exits program)

   4. if "Fruit" does exist:

   - add the fruit to next available row in CSV
   - continue with program

3. if the fruit does exist in the CSV:
   - search the fruit name on taste.com.au (web scrape)
   - Look at the top 3 (Non-Featured) recipes and identify which has the most ingredients
   - Store the Recipe name in Column B next to the relevant fruit
   - Store the Ingredients in column C, separated by a new line with no excess white space
   - Prompt the user to ‘Start Again’ or ‘Exit’

**Submit your project folder and completed excel file in a .zip.**

**If you have any issues with any of the steps, you may simplify where applicable. I.e.: if selecting the top 3 recipes is too challenging, select any single recipe.**

What's being tested?

- managing control flow and logic
- sanitising inputs
- working with API's, sanitising responses
- web scraping
- automation with UIpath

Do a full writeup of my interpretation and solution to the test and how to run my solution
list extensions and libraries used
