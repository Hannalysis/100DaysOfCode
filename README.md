# -100DaysOfCode_Challenge
Challenged by SoC. Challenge accepted!

--- Day 1 ---  
 2024-10-17

After recently completing my pre-course bootcamp material for SoC, I've discovered that I'm not that confident with CSS.
So today I focused on the materials on The Odin Project, learning about Flexbox.

I wanted to improve my knowledge by starting to go through the exercises for flex under the foundations folder within the css-exercises provided.
Today I completed exercises _01-flex-center_ & _02-flex-header_.

I struggled a bit with the 2nd exercise; I did a fair amount of trial and erroring many flex options inside different containers, and using the DevTools to inspect to try and figure out what styles were being used or overwritten.

------------

--- Day 2 ---  
 2024-10-18

Continuation of the flex exercises from the css-exercises from The Odin Project; _03-flex-header-2_ and _04-flex-information_.

The first exercise went well however the second one took a considerable amount of time - just when I thought I got a better grasp of grouping containers I had a bit of trouble aligning the text appropriately under each image item. 
It took me a while to realise I needed to make seperate containers for each item and text, and then justifying those into columns themselves.

------------

--- Day 3 ---  
 2024-10-19

 Today I wanted to divide my time; begin with a little css practice, and move onto continuing my python coding journey to improve my logic and algorithm thinking!

 Started with another flex css-exercise from The Odin Project, _05-flex-modal_. I spent time planning the containers & row/column divides I would need for this to work. 
 This has been the first time since using CSS where I felt like I was inputting style with intent, rather than almost pure trial and error.

 Ended the day with a revisit to an old quiz terminal app I had created a couple of months ago (kudos to Angela Yu's python course on Udemy).
 Until today, the questions were hard coded into a separate file saved locally. I am now using an API call request to the Open Trivia DB site to grab a random set of 10 boolean questions to print and answer inside the console.

 However, there was a small issue present as the HTML escape entities were also being printed within the questions, so I needed to import the html module and utilise the unescape function so the characters are translated back to their original form.

 ------------

--- Day 4 ---  
 2024-10-20

 Much like yesterday, today I wanted to again divide my time between css and python.

 From css-exercises I completed _06-flex-layout_, this one took a bit longer than previous exercises due to it being an entire page to layout. I encountered a little 
 difficulty with the footer positioning until I realised 
 that adding the rule _justify-content: space-between_ in the main container solved that issue.

 I then added the GUI to the python Quiz App I was working on yesterday using python's tkinter. This code has been placed into a seperate file under it's own class to 
 initialise the GUI for the app, and the class is imported back into the main file.

 ------------

 --- Day 5 ---  
  2024-10-21

Today I completed the last exercise inside the flex folder of The Odin Project's css-exercises; _07-flex-layout-2_. I found it challenging and it took me a good while to bring the page to the desired solution's state.

I got very caught up in trying to display the boxes of text so they aligned with the same gap down the centre of the main content's container. Once I had realised the individual text boxes all required a massive width extention, they all lined up perfectly.
I also had a little trouble getting the sidebar to actually take up the entire space on the left hand side (minus header and footer); I found the solution was creating a container for both the sidebar and the content on the right to align with it, and used 
the flex-grow rule to push it and surround the main page, stopping at the footer.

 I rounded off the day with some python by inputting functionality into my Quiz App; managed to get the GUI to display the questions grabbed from the API call request. Tomorrow I am hoping to add the rest of the functionality.

  ------------

  --- Day 6 ---  
   2024-10-22

 Today I wanted to fully focus on python to finish off the Quiz App using tkinter. 

 I started with giving the user feedback inside the App when they got a question right (by showing green in the canvas), and red when they did not (by showing red). I also utilised the after() method from the window class to give enough time to show the user whether they were correct, before resetting the canvas to the original colour. 
 I also needed to move my get_next_question function inside the after method argument, as it was no longer triggering once I had moved some of the functionality to the GUI. 

 Next was getting the score counter to work inside the GUI. I nested the functions to check whether another question needed asking (still_has_questions()), and then to give a question (next_question) inside the get_next_question function.
 This meant that if another question was going to be asked, then it's a good time to update the score counter, so I added a config to the label using an f string for the score number to update in.
 
 On the other hand, if still_has_questions remaining was False, I added a line to config the canvas to inform the user with text to announce that the quiz is over. Followed by disabling the buttons on the GUI to make it clear that the quiz is finished.

 ------------

 --- Day 7 ---  
  2024-10-23

 I started the day with reading up on API calls to get a better overall understanding (with python). As there was little actual coding on my part, I decided to come back to my CSS learning via The Odin Project site curriculum; meaning, we're onto the CSS project!

 Which, means practicing the CSS will come later as I needed to create the index.html file first, from scratch. So,  I spent the rest of my time populating the content in HTML, including high-level containers and a few mock-up images I made quickly in MS paint. This part has been pushed to my newly made repository (odin-landing-page).

  ------------

 --- Day 8 ---  
  2024-10-24
 
Today I decided to continue the odin-landing-page CSS project, by focusing on the CSS. 

I prioitised adding all the font rules, colours and backgrounds (while adding a couple of extra containers along the way), and pushing those changes, before heading into the flexing shenanigans.

I started with what I thought was the easiest part - sorting out the 4 images with text in the middle. I managed to get them aligned appropriately, but I do need to sort out the overlapping text. I moved onto the quote section and got that in a reasonable space as it was mostly text align and background padding.
The call to action section, is causing me a little bit of formatting issues, however I've managed to centre it, place it 2 out of 3 elements inside a box with curved corners; and will continue tackling this section next time. 

  ------------

 --- Day 9 ---  
  2024-10-25

Much like yesterday, today I wanted to continue working on the CSS project. 

I started by adding more containers, to then flex the items to the best of my ability, and also made a fair amount of margin, padding and gap alterations as my page started to take a better shape. I then realised my entire page was looking extremely elongated (partly used to using a widescreen monitor) however, 
I could negate this by adding margins to each of my main container blocks (by using padding on the left and right of each container), and made the content appear more portrait. 

I managed to get the page in a good enough state to complete the exercise, and it's an active webpage on github here https://hannalysis.github.io/odin-landing-page/ 
This by no means I'm done with it, as I expect once I have gotten more web dev experience I would like to come back and make the final tweaks to mimic the original image.

One thing that stood out to me in particular, is how convoluted some of my naming conventions were for my containers. Ones which had a couple of containers in containers, were pretty self explanatory and thus easier to label but with my 'awesome' section got very messy quite quickly. I had to keep checking on 
multiple occasions which container had what in it, and whether I had worded it correctly inside the stylesheet (as my labelling had become a little inconsistent). This is something I will pay more attention to in future projects going forward.

  ------------
  
 --- Day 10 ---   
  2024-10-26

 I wanted a well-earnt break from CSS, so I started today with reading and watching some python tutorials. My first takeaway was knowing and understanding the 4 different types of API calls/HTTP request types:

Get - _requests.get()_ Ask --> Response

Post - _requests.post()_ Send data --> Response (mainly confirmation)

Put - _requests.put()_ Update data --> Response (mainly confirmation)

Delete - _requests.delete()_ Delete data --> Response (mainly confirmation)
 
Outside of this, I came across the  _strftime()_ method. This converts a date & time object into a readable format by passing in a string, which is an essential tool for future python projects, especially for any data analysis.

I then finished my day by getting more familiar with Javascript, and completed the Rock-Paper-Scissors project from The Odin Project, under the [odin-rock-paper-scissors](https://github.com/Hannalysis/odin-rock-paper-scissors) repo

  ------------

 --- Day 11 ---   
  2024-10-27

  Today I focused on my python course in Udemy. The section I'm now on is actually focused on web development so ended up being a useful test my knowledge day (and ironically, no python at all!).

  The first project was a revisit (for me) to basic HTML (similar to the initial odin-recipes project). I did appreciate having a reason to add horizontal rule elements to this, as I had no yet found a reason to utilise one previously.
  I was also made aware of the 'vscode-icons' extension, which has made locating files more visually pleasing.

  The second section I covered lists, including nested lists, anchoring, and also attributes you can add into lists (ie the 'start' attribute, where you can start an ordered list from any number set). 
  This was then practiced into the second HTML project, including images using web links as the source, as opposed to local ones.

  ------------

 --- Day 12 ---   
  2024-10-28

  Alike yesterday, I continued with the web development section inside my python udemy course. Now we're moving onto CSS; a chance to revise, and learn something new.

  I started with a basic website project that utilised styling with just ids, classes and element selectors. I did also learn of a new selector type, called attribute - using square brackets, can select everything with the same attribute type, specific setting or, targetting items without that attribute 
  (ie p[draggable = "false"]).

  Font size measurement reference:  
  Static sizing: 1px = 1/96 inch | 1pt = 1/72 inch  
  Relative sizing: 1em = 100% parent | 1rem = 100% root

  In the second project (creating a web meme), I utilised my first custom font utilising fonts.google.com, and establishing a reference in html, using the preconnect relationship attributes, with a url link to the font in question.
  This was also the first time I've really seen the advantages of using percentages of widths and margins to make aligning content more straightforward, along with using relative font sizing.

  ------------

 --- Day 13 ---   
  2024-10-29

  Today I continued with my python course, and had my first look into web scraping. 

  I started with an exercise scraping a local html file, with the module beautifulsoup4. I was able to understand how to scrape by using the find and select functions quoting the tags from the html in order to print that information into the console.

  The second exercise, focused on using a live news website, where I was required to use code to first grab the first article, and its link, and upvote number. I had to do the same with the page of news, where gathered information was stored in separate lists, thanks to a for loop and a bit of list comprehension.

  I then finished up with writing code for printing out which article was the most popular. Utilising the max function and the index number from the upvote list I was then able to use that index in the article name list to print the relevant information.

  ------------

 --- Day 14 ---   
  2024-10-30

  Today I continued looking into the web scraping tools in python, and completed my own project - scraping the top 100 games of all time from empireonline, and printing out the list into a text document.

  Overall the project went pretty smoothly; it took me a little while to figure out the list comprehenion I needed to remove the html tags from the original printout inside the terminal, mind. 
  Once I had the list printed out with strings only, it was a matter of using the _reverse()_ function (so the listed printed from 1 instead of 100), and then using the _write()_ function in a for loop to place the items into a list with a new line (/n) spacing.
  I had to make a condtional as the write command has multiple modes; one for making a new txt file, and one for editing it, so I made it so the write iteration only passed through the once, and then took the main loop code after (by using i increments).

  ------------

 --- Day 15 ---   
  2024-10-31

  Today ended up being quite eventful, so I decided to continue with a bit of web scraping practice - this time, scraping the top 100 songs from a certain week in history.

  This particular site was a little was a little difficult to read, as the class names are extremely long (and also contain all font elements as part of the class name). I also had to do multiple separate scrapes, one for tha songs, and another for the artists...minus the no 1 song for that week.
  That was due to the fact that the no 1 song and artist name had their own class name, and visual representation on the site different (likely to make them stand out more).

  I then made two list comprehensions to clean the lists, then utilised the string _insert_ method to place the top artist and song as the first item in their respective lists. I hope to make the final touches of this project tomorrow.

  ------------

 --- Day 16 ---   
  2024-11-01

  As mentioned in yesterday's entry, I decided to continue my python project scraping the top 100 songs from the billboard website.

  To give my script more use cases, I added an input function to ask the user to add any date in the format YYYY/MM/DD (including the '/' characters). To get the date in a compatible format to fit as part of the website link, it needed to go through a bit of a conversion process.
  
  Firstly, I required that output to become a tuple - so I used the _map_ function, which encompassed an int conversion of the initial input variable (with a split to remove the '/'), all inside a tuple type conversion assigned to a new varaible.
  Then I had to convert it into a new variable as a date object (with the _datetime_ module), and assigning the individiual elements of the tuple to it.
  Finally, I inserted this new variable into my request string as an f string, replacing the part of the link where the date was being called.

  As a finishing touch, I converted the song and artist lists into one dictionary using the _dict_ and _zip_ methods, and using similar code as I did in day 14, looped through each item of the dictionary into a text tile. The filename also included the date variable from the input method (using another f string), for clarity. 
  A minor issue with using this loop for the dictionary is that the text file includes parentheses characters around each key pairing. I'll put this as a small TODO to tidy up tomorrow.

 ------------

--- Day 17 ---   
 2024-11-02

  I started the day by seeing if I could tidy up my text output from yesterday's project. After 20 minutes of looking up and trying various methods, I realised I called the variables inside the f string as a key value pairing! 
  Once I separarted the key and value into their own curly brackets, the parentheses were omitted in the text output:

  f"{song, top_one_hundred_songs[song]}\n" **-->** f"{song}, {top_one_hundred_songs[song]}\n"

  I then spent a surprisingly large amount of time trying to install node.js on my windows machine. The environment seemed to only work per launch of powershell, so it took additional research, and guidance from a fellow web dev.
  Managed to get to node and npm version checks to register upon each launch without manual input once a solution was found for the env, so calling that a win for the day.

------------
  
--- Day 18 ---   
 2024-11-03

 Today I started with continuing the javascript materials in the Odin Project Foundations course...which ended up having some downtime due to Git Bash environment setup. I needed to make sure Git Bash could locate where node was installed and appropriately linked the path in the windows 
 environment settings.

 After that ordeal, I forked the javascript-exercises repo and worked through the first 3 exercises. This included getting familiar with the test scripts in javascript.

 ------------
  
--- Day 19 ---   
 2024-11-04

Today I spent my time sorely on exercise 4 of the javascript-exercises; _04_removeFromArray_.

I managed to make a function that allowed a singular numeral argument as the element that needs to be removed, however that answer was not scalable.
Once I realised I required the ...args argument so the function could accept more optional arguments as input, is where my code got tricky (especially as I use utilising a loop for the item removal, and the splicing method, which ended up with multiple loops).
After an embarassingly long amount of time trying to get all the tests to pass, I decided to check the solution. More javascript practice to follow.

 ------------

 --- Day 20 ---   
  2024-11-05

  Today I continued with the javascript-exercises from The-Odin-Project. I managed to complete _05_sumAll_ and _06_leapYears_ with no issues.
  I can almost say the same for _07_tempConversion_, however I did have to take a bit of time to locate what method I should best use to round the numbers (using round did not allow me to specify any decimal places, 
  so I utilised the toFixed() function, with a parseFloat type conversion to get the desired output.

  After that, I read up up on the following section, DOM Manipulation and completed the first exercise; checking I am able to utilise javascript to populate html elements and append them appropriately inside their containers & divs.

 ------------

 --- Day 21 ---   
  2024-11-06

  Today I continued my efforts on learning more javascript via The Odin Project Foundations course. Starting with a continuation of the DOM learning materials, and learning about Event elements.

  As the next part required me to update the odin-rock-paper-scissors repo, I had to learn and understand how branching works in Git, and created a branch for the UI update I'd be doing to the project.
  I managed to add functional buttons to the HTML, which triggered the round and selected my choice appropriately. I also started commenting over redundant variables and functions I'm no longer calling, and made a PH div through the DOM so I should be able to 
  flesh out the results into the UI instead of the terminal tomorrow.

  ------------

 --- Day 22 ---   
  2024-11-07

  As mentioned yesterday, today I continued my efforts on revisiting the odin-rock-paper-scissors project.

  I managed to utilise the DOM to change multiple div elements to reflect the selection, round and overall score which refreshes on every button click. I'm beginning to see the similarities between javascript DOM and Python's tkinter GUI module.
  I then deleted the redundant playgame() function, and any other code I had commented out that was no longer serving any purpose. Once I was done with the updated game functionality, I gave myself a victory lap by adding some basic CSS
  so the game is more visually pleasing inside the browser.

  Finally, I pushed these files into my new branch, and learnt how to merge files back to main in Git, and delete the now redundant branch. The completed project can be viewed on this page: https://hannalysis.github.io/odin-rock-paper-scissors/

  ------------

--- Day 23 ---   
 2024-11-08

 After a week of full-on Javascript related learnings, I decided to return to my Python coding journey today. I started by practicing on the area I had left by completing a small web-scraping project utilising the BeautifulSoup4 module, on a static site.

 I attempted a similar approach to a live site, with many headers to assist with the request, however I was unable to get through the captcha prompts.
 Then I moved onto learning about the Selenium module, and utilising that I was able to access and print the information I was after.
 I intend to continue exploring the Selenium module tomorrow with exercises inside Day 48 of the Udemy course.

 ------------

 --- Day 24 ---   
  2024-11-09

  Today I decided to continue to familiarise myself with the Python module, Selenium. One of the exercises involved practicing utilising the _XPATH_ technique and _find_elements_ function to pull data from a heavily nested html element with little unique identifiers.
  Once I grabbed those, I needed to convert the web elements to make them readable with the .text function, and used this inside a loop to place the two lists of scraped data (of dates, and events) into a nested dictionary (_event_dict_) with indexes:

  for i in range(0,len(event_names)-1):  
    i_dict = {}  
    i_dict['time'] = event_dates[i].text  
    i_dict['name'] = event_names[i].text  
    event_dict[i] = i_dict  

 ------------

 --- Day 25 ---   
  2024-11-10

  More Python; so therefore more Selenium practice! 
  I started with a simple scrape to wiki to grab the amount of English articles, and utilised the _click()_ function for the first time - which took me to a different webpage without a manual input.
  With that and the _send_keys_ function, I had to then follow-up and complete an exercise to autofill out a dummy sign-up site simply by running the script.

  I also found out a way to automate a key command selection (ie ENTER) by importing the Key class from the Selenium module, however I am yet to utilise it's function in practice yet - so will likely be looking at this tomorrow!

------------

--- Day 26 ---   
 2024-11-11

 So today I started working on a project to test my knowledge on the Selenium module - making a script to automate playing a version of the Cookie clicker web game (the one at orteil.dashnet.org).

 I encountered struggles from the get go, as I spent a little too long trying different approaches to locating the html elements, only to find once I utilised input functions to pause and resume the script, the code was locating those elements fine, its just that the script was
 not allowing for web page loading times - including the times between pop-ups such as cookies, and language selection. I added a command to halt the script briefly, and it allowed my script to dismiss the prompt and select the locale.
 I originally utilised the _implicitly_wait()_ function from the _WebDriverWait_ class however once I realised it activates once per script, it was not effective enough for script to execute each command successfully. The function to click the cookie was not working, unless I paused the script manually.
 I'm going to explore more options tomorrow, experimenting with the _time_ module, which has more flexibility, and hopefully, we can get a loop of clicks implemented too.

------------

--- Day 27 ---   
 2024-11-12

 Today I continued with my automated cookie clicker script in Python, using Selenium.  
 
 As mentioned yesterday, I managed to utilise the time module to allow coding executions to await appropriate site loading, and again awaiting the game interface to load properly once getting through the initial dialog boxes.
 I got the code to loop, and managed to execute the clicker for 5 minutes, with simple hard coded int conditionals to allow for automatic upgrades to be selected within that loop - however that does not scale well.
 I then decided to scrape the elements that check the upgrade increment cost, however, despite converting the variables to int, the conditionals did not like the thousand comma separator for the 3rd upgrade. The strip method did not resolve it either, so I'm going to investigate this tomorrow.

 ------------

--- Day 28 ---   
  2024-11-13

Today I finished up my cookie clicker project.  

It came together quite quickly once I realised I could utilise the string replace method to remove the comma separator, and then convert that result into an integer. Therefore I was able to create a variable that located the current upgrade cost, 
and converted it into an int that could be compared to the cookie funds we have to spare, and picked the most expensive upgrade it could afford. 
I also placed the replace methods on the upgrade variables that do not initally require it, however if I wanted to expand the length of time I wanted the code to execute (ie 30 mins instead of 5) 
then the code would still execute without once the smaller upgrades reached 4 digit figures.

I finished up the day by looking at my next project inside The Odin Project Foundations course - the Etch a Sketch.
I got the repo made, documents created and ended with a small loop of code inside the javascript, populating 16 div elements inside the html file.

------------

--- Day 29 ---   
  2024-11-14

Today I continued my efforts on the Etch a Sketch project, and pushed my changes here: [odin-etch-a-sketch](https://github.com/Hannalysis/odin-etch-a-sketch)

I improved my initial grid generation loop; rather than spitting out 16 boxes in a line, I madea a nested loop to generate 4 boxes inside another div, named row -
which would also run 4 times in total for the 16x16 grid. I then made the rows flex to make the grid form appropriately, and added basic visuals to the boxes
so they could be seen.

I followed it up with the next step - adding colour trails to the boxes with hover and the _addEventLister_ function.
I initially got it running by accessing the div elements...however I realised it was also targetting the row divs (visually would have been passable however I curved my box edges so it was obvious). It took a while to get the code running when I switched out div for class name, as the addEventListener 
refused to run against an HTML collection object. So I had to create an array to pass through each html item, and then code worked as intended!

------------

--- Day 30 ---   
 2024-11-15

Today, much like yesterday, I continued to work on the Etch a Sketch project, and pushed my changes to the repo.

I created an input button that would allow the inputted number to generate a n x n grid inside the browser page. However, the issue arose when I created a gridClear function that did not clear the entire grid.
It took a while to realise that making a for loop to iterate through each element of the HTML collection was fruitless as the deleted elements would push the items up the list and the loop would miss them.
So I had to create a const for the collection length before the loop iteration, and that allowed the previous grid to be fully deleted before creating a new one.

------------

--- Day 31 ---   
 2024-11-16

Today I managed to complete the Etch a Sketch assignment from The Odin Project Foundations course, with some optional extras. Link to page here: https://hannalysis.github.io/odin-etch-a-sketch/

First I ensured the input prompt would not allow figures over 100 for the Grid generation, and then spent a fair amount of time figuring out how to stop my grid overflowing outside of the allocated container space.
Turns out, I had set a dedicated size for the boxes a couple of days ago, once I got rid of that and utilised flex appropriately, no matter how big the grid was, it was contained within the allocated space.

With the initial project completed, I wanted to see whether I wanted to add in the optional extras (after first tidying up my page visually, aligning the button and giving an all-round margin on the container).
I had a look at the transition and opacity functions, and with some minor timing adjustments I added them to the grid, to make the generation functions feel more fluid.

I then looked into creating a random colour function, and replacing the original colour change, to that inside the _boxTrail()_ function. It worked well, however I personally preferred the previous trail - so I thought, why not give the project a way to toggle it?
I reverted the colour change from the original _boxTrail()_ function, and made a new function; _boxColourTrail()_ which does use the colour randomiser. 
As I now required more control and flexibility of the trails, I had to remove _boxTrail()_ from the _newGrid()_ function, and make a conditional to choose which trail to pick after the user enters a valid grid size.

------------

--- Day 32 ---   
 2024-11-17

 As I'm near the end of The Odin Project Foundations Course, I decided to carry on with that today.

 I started with reading through the Objects section, and then continued with the outstanding javascript-exercises I had forked back in day 20.
 I completed the _09_Palindromes_ and _10_Fibonacci_ exercises with only minor struggles (the syntax, as stated by Andy Harris - learning the second language is the hardest, and I'm living that experience right now!).
 I encountered more issues with the _08_calculator_ exercise. In particular, the section where I needed to utilise the _reduce()_ method. I knew I needed it, I just took a while to put it together, and something about the syntax utilising the => is not clicking with me as well as it should.
 For more logical based reasons, I did also take awhile to figure out the factorial method. I will aim to complete the remainder of the exercises tomorrow.

 ------------

--- Day 33 ---   
 2024-11-18

 I started the day with completing the remaining javascript-exercises, and then set up my repo for the last assignment in The Odin Project Foundations Course; The Calculator Project!

 I didn't run in any issues with _11_getTheTitles_, however I spent a painful amount of time on the last one, _12_findTheOldest_.
 I knew I needed to utilise a reduce method, but I could not get the code to run successfully with it. I need to do some extra study on those methods (_reduce(), filter(), map()_).
 I decided getting the solution with a longer method is better than just checking the solution, so I used syntax more akin to Python, and treating the array like a dictionary, for example:

         age = people[person]['yearOfDeath'] - people[person]['yearOfBirth'];
        if (age > savedYearsOld) {
            savedYearsOld = age;
            savedPerson = people[person];
In summary, using square bracket pairings to step into each data value pairing. My solution was longer than what was provided, however I was pleased I did manage to get through the test cases with that code.
      
------------

--- Day 34 ---   
2024-11-19

Today I started working on the odin-calculator, and pushed my current progress to the repo, here: https://github.com/Hannalysis/odin-calculator

I added the initial functions; some of which have come directly from the javascript-exercise on calculator on Day 32.
I then spent a bit of time working on my first switch case loop, and using that as my method for the _operate()_ function.
The main issue I was having was that I was returning 'undefined' when utilising my console.log tests, and realised that I had written the case statements incorrectly,  
ie  _case operator == '+':_ instead of simply  _case '+':_  
So I was in fact making boolean results which would not return a correct value type once the code had executed.

I also created a couple of const to utilise the unicode for the multiply and divide symbols, which should aid me in creating my visual
calculator in html tomorrow.

 ------------

--- Day 35 ---   
2024-11-20

Today I continued working on the odin-calculator, focusing on the display.

Therefore I decided to re-use the code I had made from the etch-a-sketch; the nested loop to generate the boxes inside the row elements utilising the DOM. The main difference this time, is that rather than just creating boxes of a shared class, I also added a bespoke id to each box by
adding template literals to each name with the iterator to make them unique.  

My struggle today came with trying to manipulate the created boxes on the top row - to remove all but one box, and push it to fit the size of the other rows to mimic a calculator screen.  
I made the other boxes on that row 0 width and height, and attempted to flex grow the remaining box, however that did not work. I followed the devTools suggestion and ensured the parent container's _display:block_ & _display: flex_ was enabled. I then tried a similar idea but with removing
the other box elements with _display:none_ however I still had the same issue. For now, I decided to work with the _display:none_ and manually made the width of the remaining box a hard-coded width so it looks appropriately stretched like a screen and meets the edges of the other DOM generated buttons.

 ------------

--- Day 36 ---   
2024-11-21

Today: More work on the odin-calculator!

I started with changing the method for creating text on the div for the calculator buttons; I edited the code to create and append a paragraph html element, followed by the innerHTML on the paragraph variable to display the text. I then changed that hard-coded text to a variable that iterates through a list
of calculator buttons (including the const I had made for multiply and divide a couple of days ago). The first 3 elements of the list, are just dummy elements, as the first 3 boxes of the calculator grid generation are hidden (as mentioned yesterday). I've made that clear inside the code with a comment and labelling those
elements as 'N/A' strings for clarity.

With the visuals complete, I started work on the functionality of the calculator, starting with button execution. I added an _addEventListener_ method to the calculator generator loop so every button would have a click functionality on the p element (and for now, prints the digit/symbol inside the console log).
I then created a bespoke _removeEventListener_ on the first viewable box(aka box4, the calc display) as I did not want the user to be able to click on the calculator screen.
However, I noticed if I clicked outside the paragraph element (which only took up 50% of the box) the console.log would print that div html element (the parent info). So I edited the CSS; flexed the div boxes and added _flex-grow:1_ to the paragraph elements (with no margin) so they took over the entire div 'button'.
Due to the flex changing the location of the text, I had to adjust those elements by adding an _align-content_ rule inside the div box, and a small _padding-top_ on the paragraph*.

\* Note: There is still a minor bug present here; if I click on the very edges of the button, the user will click on the div instead of the p element, and will print a full html element.

------------

--- Day 37 ---   
2024-11-22

Today, I've made a lot of progress with the odin-calculator project - fully functioning, just needs a few adjustments that I'll hopefully complete tomorrow!

I started with fixing the bug I found yesterday. Using the _replace()_ function, I started with this:

    cleanTargetDigit = targetDigit.replace(/<p>/g, "");
    screen.push(parseFloat(cleanTargetDigit));

The above was enough to fix my bug, due to discovering that interestingly parseFloat manages to grab the float number from the left hand side of the string, and ignores the rest. 
However, in case I wanted to take the clean String variable I decided to change it to the below statement, after realising you can make an or (|) statement inside the argument parameters:

    cleanTargetDigit = targetDigit.replace(/<\/p>|<p>/g, "");

After that, I moved onto adding the remaining functions required: _operatorClick()_ (which I added to the DOM calculator generator loop), _clearScreen()_, _updateScreen()_ and _calculate()_ (for the returning value to be updated on the calc's display).

------------

--- Day 38 ---   
2024-11-23

Today, I can finally say I've managed to complete the odin-calculator project to a satisfactory state - for now. Page located here: https://hannalysis.github.io/odin-calculator/

Admittedly, this is the first time where I've gotten a little frustrated with attempting to write code when I felt like I knew where and what I wanted to write, but due to my lack of javascript knowledge I was struggling to locate the method I needed to get
the ongoing calculations to function as long as the current screen had an operator inside of it. I focused on boolean style functions, first _search()_ (then I realised that was a string method but my screen is utilising an array), and _indexOf()_ (just did not work outright with the code I had). 
I also got bogged down too much into trying to find a method or a way to set a value using newReg with the operators I needed it to search for. After a much needed break, I finally managed to create a function using the _includes()_ method, and simply used the or comparison operators to iterate through them.
This worked out well as I needed a way to flag the opposite functionality of no operators present (at the start of the calculate function(), so if '=' is selected with no operators, no calculations will occur). 

Outside of making the calcuator less bug prone, I also added a couple of keyboard funcitonality buttons - clear on DELETE & Backspace, and = on ENTER (just realising...I pushed my commit msg saying that I'd assigned Backspace to ENTER!). I considered adding the same keyboard functionality to the digits and the operators
however due to how I'm populating the calculator and the EventListeners inside the calculator generator with DOM I would require many bespoke functions that almost mirror the click versions. So I'm postponing that for a later date, when I refactor my calculator to utilise a bespoke calc class.
I also went against the extra credit task for disabling buttons, as I'd already done that off of my own back as my personal extra credit work on the odin-rock-paper-scissors project.

Finally, I added a little bit more CSS; darkened the operator buttons, added a hover to brighten the text on the buttons, and added my first _linear-gradient()_ function to the screen to give it a little shine effect.

Overall, I'm surprised how much I have learnt from doing this project, and it was a lot more time consuming than I had expected! I had completed a calculator project previously in Python but it was a small terminal app only, so I initially misjudged this project's difficulty and invested hours required. 

------------

--- Day 39 ---   
2024-11-24

With the Odin Project Foundations Course finished up and 1 day before bootcamp starts, I thought I would take a much needed Python day.

I was relieved to feel that the syntax still felt familiar, however the same could not be said for the module I was utilising - BeautifulSoup4. Carrying on with my Udemy course, I started the capstone project - 
which meant not only getting back into the swing of things after my longest time away from Python since I started learning it (10days!), I had not used that module since (looks back) Day 23 on here!

That aside, I began my web-scraping project with another static-site; this time, to grab 3 sets of information from a rental property site: links, prices and addresses from a particular filter.
The initial scrape was not too difficult, however removing all the html elements took a good while.
In particular, the address list scrape:

    addy_list = [place.getText().strip("\n\t ").replace( '|', '') for place in property_address]

 Getting rid of the pipe symbol was tricky. Whether or not I placed that symbol with spaces or no spaces, or by making another variable utilising the addy_list...it was just stubborn. So as shown, I went with a separate replace method, and that solved the issue.
 The strip list was also surprisingly long for the price list, however caused me less issues than the above.

 With those 3 pieces of data neatly cleaned and stored via list comprehension, I'll be ready to continue this tomorrow (unless I have some homework to do!).

 ------------

--- Day 40 ---   
2024-11-25

I am knackered today - I did not sleep well, and it was my first day at bootcamp! It was a great intro day though! However, I did not have a great deal of energy left post prep work so the update is not as substantial as usual.

Anyway: Continuing with Python!

Today I was far enough in the capstone project to utilise the Selenium module, to manipulate the form fields and input PH text into each cell, submit the response form, and select the option to fill in another response. My only small hurdle I encountered at first, was the realistion to also import the time module so I could add a natural wait time
to pause the script to allow the webpage to load, before actioning the webdriver functions.

------------

--- Day 41 ---   
2024-11-26

Feeling a bit better today, but I did spent a lot of time today finishing up todays work at bootcamp.
Finished up hacking an LLM task, and did many tough exercises about Git here: https://learngitbranching.js.org/

Luckily my Python capstone project; Data Entry Automation was almost complete - I managed to write my loop to iterate through the 3 list types, to autofill out in the correct fields of the google form.
The 44 entries were completed in under a minute thanks to the script, and I was able to push that data into a google spreadsheet. Feels good to finally get back into the Udemy course and complete a day again!

------------

--- Day 42 ---  
2024-11-27

Full lecture & group assignment day at bootcamp, lots of talking and with start of totm; I'm shattered!

So instead of starting a new project in Python I thought I would get through more of the exercises in CSS diner: https://flukeout.github.io/
and I managed to impress myself with my progress; from exercise 16-29. Only 3 more left, but I'll take them another time.

------------

--- Day 43 ---  
2024-11-30

Two days 'missed' due to hackathon at bootcamp. This may be a growing trend every Thurs-Fri for the next few months.

Today, to help prep for next week's lectures, I focused my efforts on the basics of Javascript, and have therefore started the Javascript Syntax Part I module at Codecademy - my first section/track (Building Interactive Websites) towards their Full-Stack Engineer Career Path.
I completed the first set of lessons and a half, covering the syntax, log statements, comments and operators.

------------

--- Day 44 ---  
2024-12-01

I decided to focus on more basics of Javascript for most of today's allocated study time.  
I completed two sets of lessons inside the Javascript Syntax Part I module; focusing on string concatenation and string interpolation (aka f strings in Python).  
I am now 29% complete on that module.  

I finished up by installing the Flask framework, and using Python to set up and run my first local web server, using the appropriate command line for Windows Powershell (only now realising that is what VS Code terminal is integrated with):  

    $env:FLASK_APP = "thefilename.py" 
and then into a separate line; flask run.

------------

--- Day 45 ---  
2024-12-02

It's been a long day, so just continued to practice and learn new javascript methods and operators.

I've realised you can add a default option to the switch case and how to utilise the ternary operator ?
I've also learnt what a short-circuit evaluation is:

    var = ''
    let newVar = var || 'not a truthy'
I'm now 35% complete on the Javascript Syntax Part 1 Unit in Codecademy.

------------

--- Day 46 ---  
2024-12-03

Today we have prep work at bootcamp that is utilising forked github repos, so taking that as my coding practice today.

I started with the object recap practice, especially getting more familiar with calling nested objects, and creating my own object of nested properties. I enjoyed also creating a nested object reflecting a bestiary monster family type from FFXI for the experimental task  
located here: https://github.com/SchoolOfCode/week-2-objects-recap-Hannalysis.

I finished with array recap practice, which was equally enjoyable. I do feel I'm more confident with creating and manipulating arrays, as they feel functionally similar to lists in Python. I decided to utilise the experimental task to utilise whole number randomizer calculations -
one for the videogame choice inside the main array, and if I picked 'Final Fantasy', the function would then initiate another randomizer and inform me which one I should play.
Second forked repro located here: https://github.com/SchoolOfCode/week-2-arrays-recap-Hannalysis

------------
