<h1 align = "center"># 100DaysOfCode </h1>
 <div align = "center"><i> Challenged by SoC</i></div>
 
 ------------

--- Day 1 ---  
 2024-10-17

After recently completing my pre-course bootcamp material for SoC, I've discovered that I'm not that confident with CSS.
So today I focused on the materials on The Odin Project, learning about Flexbox.

I wanted to improve my knowledge by starting to go through the exercises for flex under the foundations folder within the css-exercises provided.
Today I completed exercises _01-flex-center_ & _02-flex-header_.

I struggled a bit with the 2nd exercise; I did a fair amount of trial and error for many flex options inside different containers, and using the DevTools to inspect to try and figure out what styles were being used or overwritten.

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

 I then added the GUI to the python Quiz App I was working on yesterday using python's tkinter. This code has been placed into a separate file under it's own class to 
 initialise the GUI for the app, and the class is imported back into the main file.

 ------------

 --- Day 5 ---  
  2024-10-21

Today I completed the last exercise inside the flex folder of The Odin Project's css-exercises; _07-flex-layout-2_. I found it challenging and it took me a good while to bring the page to the desired solution's state.

I got very caught up in trying to display the boxes of text so they aligned with the same gap down the centre of the main content's container. Once I had realised the individual text boxes all required a massive width extension, they all lined up perfectly.
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

 Which means practicing the CSS will come later as I needed to create the index.html file first, from scratch. So,  I spent the rest of my time populating the content in HTML, including high-level containers and a few mock-up images I made quickly in MS paint. This part has been pushed to my newly made repository (odin-landing-page).

  ------------

 --- Day 8 ---  
  2024-10-24
 
Today I decided to continue the odin-landing-page CSS project, by focusing on the CSS. 

I prioritised adding all the font rules, colours and backgrounds (while adding a couple of extra containers along the way), and pushing those changes, before heading into the flexing shenanigans.

I started with what I thought was the easiest part - sorting out the 4 images with text in the middle. I managed to get them aligned appropriately, but I do need to sort out the overlapping text. I moved onto the quote section and got that in a reasonable space as it was mostly text align and background padding.
The call to action section is causing me a little bit of formatting issues, however I've managed to centre it, place it 2 out of 3 elements inside a box with curved corners; and will continue tackling this section next time. 

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

 I wanted a well-earned break from CSS, so I started today with reading and watching some python tutorials. My first takeaway was knowing and understanding the 4 different types of API calls/HTTP request types:

Get - _requests.get()_ Ask --> Response

Post - _requests.post()_ Send data --> Response (mainly confirmation)

Put - _requests.put()_ Update data --> Response (mainly confirmation)

Delete - _requests.delete()_ Delete data --> Response (mainly confirmation)
 
Outside of this, I came across the  _strftime()_ method. This converts a date & time object into a readable format by passing in a string, which is an essential tool for future python projects, especially for any data analysis.

I then finished my day by getting more familiar with Javascript, and completed the Rock-Paper-Scissors project from The Odin Project, under the [odin-rock-paper-scissors](https://github.com/Hannalysis/odin-rock-paper-scissors) repo

  ------------

 --- Day 11 ---   
  2024-10-27

  Today I focused on my python course in Udemy. The section I'm now on is actually focused on web development so ended up being a useful test of my knowledge day (and ironically, no python at all!).

  The first project was a revisit (for me) to basic HTML (similar to the initial odin-recipes project). I did appreciate having a reason to add horizontal rule elements to this, as I had no yet found a reason to utilise one previously.
  I was also made aware of the 'vscode-icons' extension, which has made locating files more visually pleasing.

  The second section I covered lists, including nested lists, anchoring, and also attributes you can add into lists (ie the 'start' attribute, where you can start an ordered list from any number set). 
  This was then practiced into the second HTML project, including images using web links as the source, as opposed to local ones.

  ------------

 --- Day 12 ---   
  2024-10-28

Like yesterday, I continued with the web development section inside my python udemy course. Now we're moving onto CSS; a chance to revise, and learn something new.

I started with a basic website project that utilised styling with just ids, classes and element selectors. I did also learn of a new selector type, called attribute - using square brackets, can select everything with the same attribute type, specific setting or, targeting items without that attribute 
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

  Overall the project went pretty smoothly; it took me a little while to figure out the list comprehension I needed to remove the html tags from the original printout inside the terminal, mind. 
  Once I had the list printed out with strings only, it was a matter of using the _reverse()_ function (so the listed printed from 1 instead of 100), and then using the _write()_ function in a for loop to place the items into a list with a new line (/n) spacing.
  I had to make a conditional as the write command has multiple modes; one for making a new txt file, and one for editing it, so I made it so the write iteration only passed through the once, and then took the main loop code after (by using i increments).

  ------------

 --- Day 15 ---   
  2024-10-31

  Today ended up being quite eventful, so I decided to continue with a bit of web scraping practice - this time, scraping the top 100 songs from a certain week in history.

  This particular site was a little difficult to read, as the class names are extremely long (and also contain all font elements as part of the class name). I also had to do multiple separate scrapes, one for tha songs, and another for the artists...minus the no 1 song for that week.
  That was due to the fact that the no 1 song and artist name had their own class name, and visual representation on the site was different (likely to make them stand out more).

  I then made two list comprehensions to clean the lists, then utilised the string _insert_ method to place the top artist and song as the first item in their respective lists. I hope to make the final touches of this project tomorrow.

  ------------

 --- Day 16 ---   
  2024-11-01

  As mentioned in yesterday's entry, I decided to continue my python project scraping the top 100 songs from the billboard website.

  To give my script more use cases, I added an input function to ask the user to add any date in the format YYYY/MM/DD (including the '/' characters). To get the date in a compatible format to fit as part of the website link, it needed to go through a bit of a conversion process.
  
  Firstly, I required that output to become a tuple - so I used the _map_ function, which encompassed an int conversion of the initial input variable (with a split to remove the '/'), all inside a tuple type conversion assigned to a new variable.
  Then I had to convert it into a new variable as a date object (with the _datetime_ module), and assign the individual elements of the tuple to it.
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
Once I realised I required the ...args argument so the function could accept more optional arguments as input, is where my code got tricky (especially as I used a loop for the item removal, and the splicing method, which ended up with multiple loops).
After an embarrassingly long amount of time trying to get all the tests to pass, I decided to check the solution. More javascript practice to follow.

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
I also placed the replace methods on the upgrade variables that do not initially require it, however if I wanted to expand the length of time I wanted the code to execute (ie 30 mins instead of 5) 
then the code would still execute without once the smaller upgrades reached 4 digit figures.

I finished up the day by looking at my next project inside The Odin Project Foundations course - the Etch a Sketch.
I got the repo made, documents created and ended with a small loop of code inside the javascript, populating 16 div elements inside the html file.

------------

--- Day 29 ---   
  2024-11-14

Today I continued my efforts on the Etch a Sketch project, and pushed my changes here: [odin-etch-a-sketch](https://github.com/Hannalysis/odin-etch-a-sketch)

I improved my initial grid generation loop; rather than spitting out 16 boxes in a line, I made a nested loop to generate 4 boxes inside another div, named row -
which would also run 4 times in total for the 16x16 grid. I then made the rows flex to make the grid form appropriately, and added basic visuals to the boxes
so they could be seen.

I followed it up with the next step - adding colour trails to the boxes with hover and the _addEventLister_ function.
I initially got it running by accessing the div elements...however I realised it was also targeting the row divs (visually would have been passable however I curved my box edges so it was obvious). It took a while to get the code running when I switched out div for class name, as the addEventListener 
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

The above was enough to fix my bug, due to discovering that (interestingly) parseFloat manages to grab the float number from the left hand side of the string, and ignores the rest. 
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

Outside of making the calculator less bug prone, I also added a couple of keyboard functionality buttons - clear on DELETE & Backspace, and = on ENTER (just realising...I pushed my commit msg saying that I'd assigned Backspace to ENTER!). I considered adding the same keyboard functionality to the digits and the operators
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

Feeling a bit better today, but I did spend a lot of time today finishing up today's work at bootcamp.
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

--- Day 47 ---  
2024-12-04

Today was an intense one; focusing on debugging exercises in Javascript utilising DevTools for the majority of the day.

This was actioned via Team Programming, so we all gave our input and took turns driving on the debugging - it was a great experience and gave us all a better insight on how and when to debug, and when to take a step back in situations where we may have over-focused on an area  
to re-evaluate the code and think of the lines we may have overlooked originally.

In short, when in doubt use console.log to track your variables, input arguments, and what is returned from functions.

------------

--- Day 48 ---  
2024-12-05

Today was another start of our team hackathon; the project, rock-paper-scissors.

As mentioned previously inside this readme file, I have previously completed the [rock-paper-scissors project](https://github.com/Hannalysis/odin-rock-paper-scissors) in javascript before. However, I took a look inside my js file inside that repo, and saw my old randomizer code:

    function getComputerChoice () {
        num = Math.random()
        if (num < 0.33) {
            npcChoice = "rock"
        }
        else if (num > 0.33 && num < 0.66) {
            npcChoice = "scissors"
        }
        else npcChoice = "paper"
        return npcChoice
      }
As you can see, this code is not giving a fully even 1/3 split selection between the choice the NPC can make. And thanks to the improved randomizer code I utilised for my game randomizer selections I created just two days ago (Day 46), I could re-use my improved logic and edit that file.
So that's what I did:

    function getComputerChoice () {
        let npcOptions = ["rock", "paper", "scissors"];
        let randomNumber = Math.floor(Math.random() * (3));
        let npcChoice = npcOptions.at(randomNumber);
        return npcChoice;
    }

But outside of this minor edit, it was an intense day of planning, and helping my team learn some of the Javascript required for our presentation tomorrow.

------------

--- Day 49 ---  
2024-12-06

Today was the presentation of the hackathon day. Busy, tiring but rewarding - mostly due to the fact that we gave ourselves adequate time to prepare for the presentation (even had time for 3 rehearsals!). We did well!

My main takeaway from a coding pov, is that I now know how to change the styling of the console inside DevTools - injecting CSS inside javascript console.logs, with %c and css properties stated as an additional optional argument.

------------

--- Day 50 ---  
2024-12-07

Today I started with the weekend prep work for next week's bootcamp. I am feeling very drained, and full of headache so I'm going to try and pace myself.

After reading through some HTML and CSS semantic layout documentation, I then had a go at the Grid Garden mini-game (https://cssgridgarden.com/) to practice the grid property functions; managed to achieve **level 24** out of 28 in ~35 minutes.
I was working through them at a pace but I required some additional time to understand the fractional unit (fr) and apply that knowledge.

After a break, I went through some CSS flex mini game called Flexbox Froggy: https://flexboxfroggy.com/, and I managed to complete all 24 levels in ~ 35 minutes. 

------------

--- Day 51 ---  
2024-12-08

Today I wanted to see if I could slot in a bit of a mixture of tasks:

I started with a recap of the DOM exercise that I originally completed back in Day 20, in order to prep for next week's bootcamp module.

I continued by looking into a learning material my mentor recommended: https://www.frontendmentor.io/challenges?type=free so looking at that, I decided to start adding some better container formatting, flex and image tidying up on my https://github.com/Hannalysis/odin-recipes
project. I decided to use a couple of pomodoros only, to make sure I had time to work on my Python project.
My main learnings from the today's CSS work was the use of the calc() function:  
           
    height: calc(100vh - 96.24px); /* full page - (content + margins + borders) */
Using this method and a bit of maths to calculate the remaining space of a page I wish to place inside a container, it gives me a template to work around and carefully sort out all the containers contained inside this container.

I finished up with re-visiting the basics of the flask Framework, understanding nested functions, and utilising the @ symbol to utilise the Python Decorator function.  
I intend to follow-up with the relevant exercise in the Udemy course next time I'm looking at this.

------------

--- Day 52 ---  
2024-12-09

I did not end up with as much energy as I was hoping for today, so after my day at bootcamp (intro to DOM manipulation | Events) 
I went for a quick javascript session in Codecademy, revising my current knowledge in truthy statements, and utilising some Ternary expressions.

------------

--- Day 53 ---  
2024-12-10

Today was absolutely packed at the bootcamp and the prep work was intense.

I spent the day with my team ploughing through some DOM manipulation challenges, and finished up the evening researching about APIs, Promises and the differences between synchronous and asynchronous code.  
I also signed up to CodeWars as requested, and completed my first 4 javascript katas; 8 kyu (9).

------------

--- Day 54 ---  
2024-12-11

Today at the bootcamp our team first tackled an escape room based around an API fetch (we almost solved it!) and followed up with a functioning app to call dad jokes from an API instead of from a hard coded array.  

After prep work, I had a bit of time to continue and complete all my initial kata challenges SoC set out for us to do on CodeWars : 8kyu (15).

------------

--- Day 55 ---  
2024-12-12

Today was our weekly hackathon start, and I spent the best of the evening coding the solution for the API fetch, and the functions to interact with the button and text inputs on the page:  
https://github.com/SchoolOfCode/week-3-hackathon-team-9-aquamarine/blob/main/fetch.js

------------

--- Day 56 ---  
2024-12-14

Yesterday was the weekly presentation day for our hackathon. After that, a mentor session and completing the remainder of the work for that module. I was spent.  
Back on it today; starting with the prep work for our module on Back-End Engineer next week.  

After understanding node.js (luckily, I had already installed it prior to the bootcamp); I went straight for the exercise material located on this repo:  
https://github.com/SchoolOfCode/week-4-importing-and-exporting-modules-Hannalysis  

It taught me how to export and import functions with javascript, how to run node commands into the terminal,  
and how to use a package.json file to run a script using the npm start command.

Finally, ended the day with a few exercises in CodeWars and ranked up: 7kyu (41), and a notch further on my Codecademy module: Javascript Syntax Part 1: 41%.

------------

--- Day 57 ---  
2024-12-15

Today I wanted a break from Javascript, so I did a little session on Python.

I continued with learning about the Flask module, and started understanding how to populate a basic local server with   
HTML elements, on multiple pages via the @app.route method.

I also learnt how to write a python decorator that counts how long it takes to run a function:

    import time
     
    def speed_calc_decorator(function):
        def wrapper_function():
            time_before = time.time()
            function()
            time_after = time.time()
            time_taken = time_after - time_before
            print(time_taken)
        return wrapper_function

To explain the above, I'm passing through a function, and before it activates, it will take a snapshot of the current time  
(in seconds since 1/1/1970). The function will activate, then I will call another snapshot of the current time, then using  basic arithmetic minus the second snapshot(time_after) from the first (time_before).

------------

--- Day 58 ---  
2024-12-16

Today at bootcamp we spent time practicing async functions, imports and working with node.js.

I spent an unhealthy amount of time working through a particular exercise, Ticket 2C, which required me to add a new quote to an object with an id generated from the UUID module, adding it to the existing array, and writing it to another file:

    export async function addQuote(quoteText) {
        // Grabbing the list of quotes
        const quoteList = await getQuotes();
        console.log(`this is : ${JSON.stringify(quoteList)}`);
        const newId = uuidv4();
        const newQuoteObject = {"id": newId, "quoteText": quoteText};
        // Adding new id + quote to the array
        quoteList.push(newQuoteObject);
        console.log(quoteList);
        try {
            const dataUpdate = await fs.writeFile(FILENAME, JSON.stringify(quoteList),'utf-8');
            return newQuoteObject;
            // console.log(dataUpdate);
        } catch (error) {
            console.error('Error writing file:', error);
        }
    }

------------

--- Day 59 ---  
2024-12-17

Today at bootcamp we wrestled with express to create our own API server handler. 

I managed to complete tasks for creating app functions for get, post, and patch with the appropriate status responses  
and data displayed. I started to struggle when it came to utilising the delete request and was unable to successfully get working code for now.
Repo activity app.js link below:

https://github.com/SchoolOfCode/week-4-building-a-rest-api-the-paige-turners/commit/62b2c4ae35ea7db11ebfb663d234cb101a60e4fb

------------

--- Day 60 ---  
2024-12-18

Today we continued to work with restful API, with a more difficult workshop! It was intense, and we got tripped up by tests that should have been passing some of our solutions (even the lecturer could not figure out why our tests were misbehaving!) 
We managed to get through many tasks, including making a successful GET, POST, PUT, and DELETE with the appropriate status code responses and message body.

https://github.com/SchoolOfCode/week-4-restful-api-workshop-the-paige-turners/blob/master/routes/astronauts.js

------------

--- Day 61 ---  
2024-12-19

Today was the start of our weekly hackathon at SoC.  

For our Rest API hackathon, I am responsible for populating our database (converting csv to json data) and providing the appropriate routing functionality for our server, as shown in the link below:

https://github.com/SchoolOfCode/week-4-rest-api-hackathon-the-paige-turners/blob/main/server/routes/weapons.js

------------

--- Day 62 ---  
2024-12-21

Yesterday was the weekly presentation day for our hackathon. So I rested after a heavy week of using Node.js and Express to create our own restful APIs.  

Today I decided to return to Python to continue learning and working on my first basic Flask app, utilising routes, much like Express in Javascript.  
My main takeaway from today's learning was that the img html tag could not utilise conventional style tags within, however I found out that using center tags around the img tag was the solution.  

I also revisited Python decorators, and I was surprised to realise that I'd never utilised f strings (string interpolation) to showcase just the name of the function.   
To achieve this in Python:  
     
    f"You called {function.__name__}"  
  
And, of course as I'm also studying Javascript it would be remiss to not also know that syntax:  
      
    `You called ${function.name}`  
  
I ended my day with a quick pomodoro on my Codecademy module: Javascript Syntax Part 1: 48%.  
This involved some practice with arrow function notation (arrow replaces function), and concise arrow notation (single line, no return, no curly braces, parenthesis on no arguments or two or more).
    
------------

--- Day 63 ---  
2024-12-22

Today I decided to complete my first Python Flask app (Higher Lower game, utilising routes for user guesses).

My main issue was trying to work out what syntax I had to utilise in order to allow user input inside the uri - and discovered int: variable_name, inside a tag:

    @app.route("/<int:user_guess>")

My second hurdle encountered when trying to inject multiple style options inside the html content, and realised separation between styling required semicolons.

I finished off my day by completing a couple of sections in my current Codecademy module: Javascript Syntax Part 1: 54%.
I got good practice defining functions with the arrow:

    const functionName = () => {
    }

------------  
  
--- Day 64 ---  
2024-12-27

After a lovely, much needed Christmas break (I did actually spend some of the evening on Xmas day drafting out my initial planning documents for my new personal project (codename CoCo)), I'm back on the coding bandwagon.  

Today was a research into data analysis modules, utilising Python. I was gifted a copy of _"50 Days of Data Analysis with Python"_ paperback, and spent most of today reading through all the fundamentals.  
I then finished up by writing up a list of tasks, and data analysis types I wanted to practice or utilise for my own future projects (Heatmaps, Piecharts, Box Plots, Line Graphs utilising Numpy, Pandas, Matplotlib & Seaborn).  

------------  

--- Day 65 ---  
2024-12-28

Today I realised I did not have the creative energy to start/continue planning for my personal projects, so I decided to go back and complete one of the previous SoC assignments from the Front-End Engineer module - on my own branch.  

So I selected the DOM manipulation workshop, and continued from tasks 3 - completion.  
Tasks 4 and 5 caused me little issue, but I was really struggling with 3 throughout [https://github.com/SchoolOfCode/week-3-dom-challenges-team-9-aquamarine/blob/hw/03-star-slider-challenge/app.js].  
It took me a while to first understand that I needed to grab the value of the slider in order to obtain the incremental changes, make a function to add or remove star symbols, and attach those to the correct element.  
At first I was attaching them to the parent element, which meant any styling was negated. As soon as I realised I needed to treat the html collection much like an array, I was able to point to the child element and attach the stars appropriately:

    function sliderValue() {
      let setStars = "";
      for (i = 0; i < starSlider.value; i++){
        setStars += "★";
      }
      starIcon[0].textContent = setStars;
    }
    
    starSlider.addEventListener("input", sliderValue);

------------  

--- Day 66 ---  
2024-12-29

Today was an interesting one, I didn't even write a single line of code - as I was planning my first personal project!  

Thanks to a little bit of time on Christmas day, I had hand-written a brief regarding what problem I'm trying to solve, with a rough but very much disney idealised brainstorm of what my project should and could contain.  

Today I focused on creating my first MVP, utilising Excalidraw for the first time. It ended up creeping into what I believe to be two milestones, so I ended up highlighting what would be appropriate for MS1 and then for my second iteration, MS2.  

I then spent some time figuring out what my main page is going to look like for the user, and took some screen captures of different elements and windows inside a couple of my favourite Digital Audio Workstations(DAWs); Reaper and Cubase 10 Pro.  
This included but wasn't limited to, their main pages when you open a music project (typically a hybrid of a mixing view, track selection with plugin effects, and timings and bars across the top), chord pad windows, LUFS meter, track list, EQ window etc.  
With this information, I made a first draft of my main page, with outlines showcasing what elements and interactables were going to be, and what the visual graph data was going to look like.  

I then run into my next conundrum; which visual graph module should I utilise and from what language?  
There's Pythons: Matplotlib | Seaborn | Plotly  
And Javascripts: D3 | Vegalite 

I need to investigate.

------------  

--- Day 67 ---  
2024-12-30

The investigation took many more hours than I had intended.  Outside of struggling to get some modules to showcase data in the format I wanted, I was also surprised to see how often I struggled to get a module to run at all...  

Python Modules:  
Overall I did not struggle with running any module from this language; I was having issues in regards to the options regarding visual data.  In the end, my shortlist was:  
✔️ Matplotlib  
✔️ Seaborn  (w/ Matplotlib - due to requiring the Bar Range graph)  
✔️ Bokeh  
❌ Plotly  

Javascript Modules:  
There were at least 3 cases (all crossed below) were a module depended on another module that is currently unstable (aka canvas), and the remaining two had multiple other dependencies, and interesting workarounds just to get them to function:  
✔️ D3  
❌ Chart  
❌ HighCharts  
✔️ Google Charts  
❌ Plotly   

I will not go into too much depth here, but I have recorded a document with the pros and cons of the available graph visualisations, and will refer to that to make my decision which one is going to be used for my personal project MVP.  

------------  

--- Day 68 ---  
2024-12-31

So, today was the day I finally could start my project! Which made me realise, for the first time I did not feel ready to code!  

Therefore I decided to spend some time in Github planning my tasks (in issues, maybe I should try the project tab next time!) writing what I thought was only ~ 8 tasks but I entered 13, and some are quite heavy and may require further breaking down later.  

Enough procrastinating was had, and I decided to work on my first project-related task: Building a basic wireframe in HTML and CSS.  

It felt like an age since I last really dealt with styling and it showed. But it was great to finally utilise flex methods with the flex-grow attribute stated in 2 separate containers, in my first situation outside of a mandatory exercise or mini-game.  I also learnt how to implement a couple of google fonts, by utilising the ref link inside of the head of the html file.  

I finished up the day by learning how to commit in Github by linking an issue to close upon pushing to the remote repository.  

------------  

--- Day 69 ---  
2025-01-02

I didn't have the best night's rest, so I started today with a pomodoro session practicing my javascript using a Codecademy module: Javascript Syntax Part 1: 64%  

After that, I started to work on populating a small scale instrument data set for my personal project, using google sheets.  
I was surprised how much information was tricky to collate, and I also had to mathematically convert note names to MIDI numbers...  
until I realised I could create a reference table in a separate sheet, and utilise the vlookup formula to populate those numeral conversions for me:

     =VLOOKUP(H3, NoteMIDIconversion!$A$2:$B$129, 2, FALSE)

I then utilised my csv to json javascript code to format my data (and subsequently, accidently learned that the period key '.' creates a nested set  
of key value pairings), so I decided to nest my note range typings using that shortcut, and lastly, reflected those changes inside my google sheet for smoother conversions in future.  

------------ 

--- Day 70 ---  
2025-01-03

Today I continued with my personal project.  

I started with creating a main js file, to import my dataset to and to add an id element to each entry.  I then linked each file to make sure they could communicate with one another, and to ensure when running the html file on a live server, it's able to log all of the data entries.  

My next main task was to begin implementing my draggable instrument items container - so I started with utilising DOM manipulation to generate a couple of rows of boxes inside that container (with hard coded PH numbers for now).  
I finished off today's work with some CSS to size and visualise the boxes to check the core generation was working as intended.

------------ 

--- Day 71 ---  
2025-01-04

I started my day with a section of Javascript fundamentals inside Codecademy, mostly solidifying my switch case functions. The following example below gives a lot of clarity and fun in explaining it's functionality:

    const toEmoticon = str => {
     switch(str){
       case "shrug":
         return '|_{"}_|'
       case "smiley face":
         return ':)'
       case "frowny face":
         return ':('
       case "winky face":
         return ';)'
       case "heart":
         return '<3'
       default:
         return '|_(* ~ *)_|';
     }
    }
   
 Javascript Syntax Part 1: 70%  

I then spent the day focused on my personal project - populated a container with instruments inside a separate div box element, and made them all draggable.  Implementing a drag feature was new to me, and I did have some teething issues upon implementation.  
The largest one being finding a solution for allowing my draggable elements to populate appropriately upon the web page initially loading: the position absolute attribute causes a strange stacking effect for all divs inside the same container.  
Until I realised I could edit the style element inside javascript, therefore upon initially loading the page the box divs would be set to position: relative until I executed the following DOM line inside the draggable event;

      dragElement.style.position = "absolute";  
  
With this, some CSS transition to smoothen the grabbing effect (and the side effect of grabbing which moves other divs adjusting to their new position), and z-index manipulation to ensure the dragged item is on the front layer, I completed my task and closed the issue via the github commit #.  
 
------------ 

--- Day 72 ---  
2025-01-05

Today was a hard day.  Lack of sleep, topped with TotM pains throughout.  

I spent perhaps too much time struggling with my project today - every time I tried to solve a problem, it actually caused more side effects.  I ended up going down too many rabbit holes for various attempts to create functionality and fluidity.  
After some struggles and then some, I settled with some functionality where I could drag and drop the instrument box into the input text field and it appropriately updated the box with the textContent, and then turning off the listening for any following drop events,  
with the caveat that when letting go of the dragging div, the object remains on my cursor until a secondary click action occurred.  This also came with further issues, where the div box would just awkwardly remain where I dropped it on the web page.  
I had to make a decision to attempt to clear this up, however I could not find a clean solution with the options I had trailed with.  I used remove() but it is understandably an aggressive dom solution, which means the box is then off the board until the page is refreshed.  
I tried grabbing positions and then using them to update the box upon mouse up, however they did not travel back to their og locations with the following code:  

    //with supporting code for every populated element
    let fullPosition = dragElement.getBoundingClientRect();
    let ogXPos = fullPosition.left;
    let ogYPos = fullPosition.right; 

    //to trigger when the mouse up event was activated
    dragElement.style.left = ogXPos + 'px';
    dragElement.style.right = ogYPos + 'px';

Eventually, I settled with using the cloning method. However, in my solution this still only allows the draggable process to occur on each instrument box once, but at least 'returns' (is replaced) to the original position:
     
    //with supporting code for every populated element
    let dragElementClone = dragElement.cloneNode(true);

    //to trigger when the mouse up event was activated
    dragElement.parentNode.replaceChild(dragElementClone, dragElement);

I'm starting to feel a bit pressured, as this is the project I intend to show to my mentor next week, and I was expecting to be further along than I am.  But I need to realise that this is part of the learning process, I will encounter these struggles, and   
being brave to showcase even unfinished/unoptimised/broken work is still worth doing.

------------ 

--- Day 73 ---  
2025-01-06

Today was a welcome return to SoC!  

We spent the majority of the day recapping on Express with an exercise fixing a Fullstack application; starting from the back end.  We made good progress and completed 3/5 core tasks.  
I then spent the evening focusing on the prep work; watching many videos on the fundamentals of DBMS, and in particular, SQL queries.    

------------ 

--- Day 74 ---  
2025-01-07

Today was another full-on day at the bootcamp, and after!  

Continuation of the basics of SQL, with two workshops learning how to action multiple different query types: SELECT, FROM, AS, WHERE, LIMIT, OFFSET, CREATE TABLE, DROP, JOIN (INNER JOIN, OUTER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN) etc.  
The evening session was further prep and recap. We also had to create our own sql database server in Render, and then install an open source management tool to test our database server; pgAdmin.  

------------ 

--- Day 75 ---  
2025-01-08

Another day at Bootcamp - time for more focus on SQL queries!  

Today we started with a murder mystery exercise that required executing multiple different SQL queries, and I can say that our team managed to work out who the brains behind the murder was :)  
We spent the afternoon on a workshop where we learnt about storing environment variables (with the aid of dotenv) and also marrying node.js with the sql package to use queries inside javascript to make requests with express.  

------------ 

--- Day 76 ---  
2025-01-09  

Today was our weekly hackathon day! We started working through initialising our project, and initialising the database using Postgres - once we had established what datasets we wanted to create and the relationships between both tables (ensuring PKs and at least one FK).  
Once we were able to populate our database (served with Render) we planned our API and express interactions ready for tomorrow morning.  

------------ 

--- Day 77 ---  
2025-01-10  

Today, was our team finishing up our hackathon, and presentation day!  

We managed to write successful RESTful Get (SELECT) and Post (INSERT INTO) API requests, with the appropriate status code responses for each table typing.  
After the day, I spent the evening finishing up the post day tasks; ready for the weekend prep work, and hopefully more work on my own project.  

------------ 

--- Day 78 ---  
2025-01-11  

Today I started with the weekend bootcamp prep work - this is focusing on learning to utilise Github's Copilot LLM.  

With this repo, [https://github.com/Hannalysis/skills-copilot-codespaces-vscode] I managed to grab a basic understanding and what settings I should toggle for a less intrusive experience (especially whilst I'm still in the syntax learning process) however, for some reason this particular tutorial focused on the online codespace in Github, which meant that I was completely unable to utilise the Github Copilot Suggestions panel, and this could not progress past Step 3.  
  
I tried allowing all third-party cookies to access Github.com on my main browser, and toggling on the "Suggestions matching public code", to no avail.  
It does work on my local VS Code so I'm going to spend some time utilising this tool against personal projects and exercises locally to improve approaching Copilot's assistance.  

I then finished off my day with a pomodoro in the Javascript Syntax I unit inside Codecademy.  

------------ 

--- Day 79 ---  
2025-01-12  

I started off my day with a pomodoro to finally complete the Javascript Syntax I unit inside Codecademy (despite the website not tracking it correctly today!).  

I've not been feeling very well today, so writing code for my personal project was a bit of a struggle. I did manage to add the appropriate EventListener to remove a highlighted InputField div onmouseleave.  
As I made PH static html input fields, I struggled to track their input values, once the draggable item had been dropped. My temp solution for now, was to push that value from inside the functionality during the drop event, into an array accessible in global scope.  
The issue with this solution is that the data will likey not match up visually if the user drops the instrument selection out of the sequence order (from top to bottom).  

------------ 

--- Day 80 ---  
2025-01-13 

I really did not feel well today.  But after a morning of resting, I got back to the learning; to catch-up on what I missed at bootcamp - learning to use Vitest.  

Using this repo as an introduction: https://github.com/SchoolOfCode/week-6-unit-testing-introduction-mac-10/tree/hw, I learnt how to setup execute unit tests, including when to check for errors ie when an invalid input is utilised.  
I also learnt the difference between the main two Test Runners (Jest and Vitest).  

------------ 

--- Day 81 ---  
2025-01-14 

Today I felt a bit better than yesterday, took it easy but focused on learning about TDD (Test Driven Development) and utilised it in today's workshop with my fellow peer.  
  
After the day at bootcamp, the prep work task focused on the 3 different types of Testing Strategies: Equivalence Partitioning, Boundary Value Analysis & Decision Tables.

------------ 

--- Day 82 ---  
2025-01-15 

Today I took a bit of a downslide slide, and it's my long day at bootcamp, so I just had to pace myself.  

Today we learnt a new tool: Playwright.  At first glance, it reminded me of a module I've worked with in Python earlier - Selenium. However, oh boy the power of this module though!  
One very welcome addition from the get go is the built-in auto wait and auto retry, and the Trace Viewer to scrub through the actions automated by the test.  

So we spent the afternoon working through a lengthy workshop, and almost completed it.  We must have done well on it as we got called up to demonstrate our findings on the later tasks at the end of the day.  

------------ 

--- Day 83 ---  
2025-01-16

Hackathon day! Today, we were tasked to write katas and complement them with appropriate testing requirements.  
  
It was great to use the Testing Strategies, Boundary Value Analysis & Decision tables to help manage what tests I would require for my two katas, damageBuff and teamWeapon.  
This is also the first project where I had to create my first custom markdown which included appropriate planning & table documentation https://github.com/SchoolOfCode/week-6-hackathon-Hannalysis/blob/main/README.md  

------------ 

--- Day 84 ---  
2025-01-17

Still feeling drained, but managed to get through the presentation today for the Hackathon mind!  

I wrapped up the day by looking into an API testing exercise with vitest, and learnt how to use expect to check whether content is being received in the appropriate type (ie array or object).  

------------ 

--- Day 85 ---  
2025-01-18

Today I've started prep work for next week's bootcamp module focus on Web development.  

This included watching a few videos surrounding CSS tips, and then I decided to complete the Grid Garden mini-game (from Day-50) in a pomodoro session.  This taught me the use cases of grid-template-columns & rows, and the grid-template shorthand, along with the  
use cases of the fr units to fill the remaining space.  

------------ 

--- Day 86 ---  
2025-01-19

Today I continued my prep work, and focused on my first Front End Mentor project - "Product preview card component".  

It took me a good couple of hours, mostly because I wanted to try and keep the CSS clean as possible - and I wanted to document any major learnings and changes I made to help me for future reference.     
I am overall very pleased with the results, and have published my finished work on a github page: https://hannalysis.github.io/Front-End-Mentor-Product-preview-card-component/  

I already feel like I have come a long way since my initial struggles with CSS (back on Day 1 of #100Days of Code), and also, I have seen improvements since my last CSS challenge I did in The Odin Project 3 months ago,    
located here for a comparison: https://hannalysis.github.io/odin-landing-page/ reminder: I should update this soon when I have the time!    

------------ 

--- Day 87 ---  
2025-01-20

Today we started our adventure into Web Development at bootcamp; aka our introduction to the React library!  

I almost completed two workshops around react: First one, more focused on the original React syntax inside a html document, and converting it to jsx; and the second one, learning how to utilise it in an app environment using Javascript.  

------------ 

--- Day 88 ---  
2025-01-21

Today was another lecture and documentation heavy discussion on React! I spent time with my teammates checking each other's understanding of many different concepts, including:  
Writing markup with JSX , conditional rendering , rendering lists, responding to events and updating the screen. Followed by prep work that included the introduction to Hooks, and how to apply functions or anonymous function calls inside the setState method.  

I finished up the day by updating my README file inside the "Product preview card component" project, and realised I had forgotten to supply the active states, so committed those changes as well. 

------------ 

--- Day 89 ---  
2025-01-22

Today at bootcamp my teammates and I worked on our first react app with vite - to implement a nought and crosses game.  

We made sure we spent enough time planning, before we initialised our project, ensured our hierarchy of components and their relative folders were setup before we delved into our jsx files.  

------------ 

--- Day 90 ---  
2025-01-23

Hackathon! We spent today getting our planning, initial React project initialised, and the static wireframe up and running.  
We then spent an unhealthy amount of time trying to get the card re-render 'flip' working, so we had to go ahead and do some research before reconvening our findings and overall solution.  

------------ 

--- Day 91 ---  
2025-01-24

Today was the Hackathon presentation. 

We focused the morning on the CSS of our React Flashcards app, as the finishing touches before sorting out our presentation content.  
I learnt that a @keyframe allows you to create an animation by defining styles at certain points in time during the sequence.

    animation: burnEffect 1.5s infinite alternate; /* Animation for burning effect */
    
    @keyframes burnEffect {
      0% {
          text-shadow:
              0 0 5px rgba(37, 68, 65, 0.8),
              0 0 10px rgba(37, 68, 65, 0.8),
              0 0 15px rgba(37, 68, 65, 0.7),
              0 0 20px rgba(96, 169, 162, 1),
              0 0 25px rgba(96, 169, 162, 0.8);
          color: #254441;
      }
      50% {
          text-shadow:
              0 0 5px rgba(37, 68, 65, 0.9),
              0 0 10px rgba(37, 68, 65, 0.9),
              0 0 15px rgba(37, 68, 65, 0.8),
              0 0 25px rgba(96, 169, 162, 1),
              0 0 30px rgba(96, 169, 162, 0.9);
          color: #60a9a2;
      }
      100% {
          text-shadow:
              0 0 5px rgba(37, 68, 65, 0.8),
              0 0 15px rgba(37, 68, 65, 0.8),
              0 0 20px rgba(96, 169, 162, 1),
              0 0 25px rgba(96, 169, 162, 0.9),
              0 0 30px rgba(96, 169, 162, 0.8);
          color: #254441;
      }
    }
------------ 

--- Day 92 ---  
2025-01-25

After finishing up with the weekly wrap up from week one of our focus on React, I decided to revisit and attempt to solidify my React learnings by taking a short React course in Scrimba.  

I decided to pick the intermediate challenge "Build a Memory Game", which is about 4+ hours of tutorials and interactive exercises on a web integrated IDE.  
I completed the first 1/4 today; which actually focused heavily on the gaming logic, aka javascript functions, but it was still welcome as it gave me an opportunity to practice using map (getDataSlice), looping to store unique numbers inside an array (getRandomIndicies), and  
learning that the Fisher-Yates algorithm is the array shuffling method (which is super handy to know for future projects I want to create!) 

    function getDataSlice(data) {
        let randomIndices = getRandomIndices(data);
        const dataSlice = randomIndices.map(index => data[index]);
        return dataSlice;
    }

        function getRandomIndices(data) {
        const randomIndicesArray = []
        
        for (let i = 0; i < 5; i++) {
            const randomNum = Math.floor(Math.random() * data.length)
            if (!randomIndicesArray.includes(randomNum)) {
                randomIndicesArray.push(randomNum)
            } else {
                i--
            }
        }
        
        return randomIndicesArray
    }

------------ 

--- Day 93 ---  
2025-01-26

Today I decided to continue my learning journey inside Scrimba; by continuing the "Build a Memory Game" in React course.  

We started to focus on the Core Game Functionality - and in particular the behaviour of selected cards.  

This involved moving certain key values from an array of objects, stripped down to an index value and a name string, and passing it through from a component lower down the tree, up to its parent to utilise inside a function located there  
(in this particular case, for the turn card function).  This was an area I really struggled to get the concept of, and visualise, so I spent a lot of time here, and I also got an explanation from a fellow software dev with experience in React to assist with the visual aid.  

It was tempting to try and get through this 'short course' as quick as possible, but I decided to leave it at 33% for now, rest and reflect on the learnings, and come back to it to continue it next as soon as I'm able to.  

------------ 

--- Day 94 ---  
2025-01-27

Today at bootcamp we focused on learning the importance of utilising methods that do not mutate the original data.  

So the focus was heavily on understanding spreading, and either removing, replacing or changing a value inside an object or array, without editing the original input.  
Our team did really well and we got to the last exercise, which I managed to complete in my own time:

    // Immutably update the array as well as the object at the given position/index within the array, so that the value under the "completed" property becomes the opposite of what it was.
    // Any other properties in the object should be maintained.
    
    export function toggleListItemCompleted(array, index) {
        let newArray = [
            ...array.slice(0, index),  
            {
                ...array[index], 
                completed: !array[index].completed
            },
            ...array.slice(index + 1)
        ];
        return newArray;
    }

and I'm also proud of aiding with this particular solution:

    // Immutably update the object so that the value under the "needsACupOfTea" property becomes the opposite of what it was.
    // Any other properties in the object should be maintained.
    
    export function toggleTeaStatus(object) {
        let newObject = {
            ...object,
            needsACupOfTea: !object.needsACupOfTea,
        }
        return newObject
    }

------------ 

--- Day 95 ---  
2025-01-28

Today at bootcamp we were tasked with a workshop that gave us the opportunity to investigate documentation and apply our findings in order to create test cases in react with the react-testing library with vitest.  
Most documentation avilable is for the similar alternative testing package, jest, so we had to establish the nuances between the two.  

Our team were then tasked to investigate nested CSS, and the differences between native nested CSS and SASS - for our presentation tomorrow morning. 
  
After the prep work, I focused on more of my scrimba course, utilising more useEffect methods.  
I wrapped up the evening by forking our hackathon on Friday for my React practice, to implement the react-flip-card library onto the Flashcard component, and then refactor that code.  

------------ 

--- Day 96 ---  
2025-01-29

Today we presented our presentation on native CSS & SASS nesting.  We also were introduced to the storybook frontend UI workshop library, which weaved nicely after a talk that was focused on user-centred design.  
We finished off the session with an investigation researching useReducer, and when to utilise it over useState hooks.  

After prep, I finished the day off with continuing React practice; by obtaining initial functionality with form submission (currently, data is stored in a variable and output is printed to the console).  
My next focus on this, is to refactor the code, and move some data and states up the component tree to allow full functioning form capabilities.  

------------ 

--- Day 97 ---  
2025-01-30

Hackathon today! We had flexibility to create anything in React, so we settled for something Owl themed (due to our team name) and decided on an Owl Quiz; where the question is an image, with a set of multiple choice answers.  
The incorrect answers would still be generated from the answer array, but excluding the correct answer text for the matching image.  Once a question was answered, the image and the buttons would be re-rendered to view a new image and multiple choice selection.  

------------ 

--- Day 98 ---  
2025-01-31

Hackathon Presentation today!  
  
We focused on small updates to our app as time is short in the morning.  We added a running score, and very basic Playwright testing (as we realised, due to the random nature of our image and button functionality, there would be additional logic to create a useful test  
that we just did not have ample time to explore with).  
  
We also added a owl hooting SFX to trigger when the user selected the correct bird. However, the original SFX itself was too long, and clipped at the end of the track - so I put my audio editing skills to use;  
trimmed down the SFX at the first hoot ending phrase, and a gentle fade out on the tail for clarity, and replaced the og file for our new edited version, and pushed up within the space of 5 mins.  

------------ 

--- Day 99 ---  
2025-02-01

After finishing up the module from the bootcamp for this week, I wanted to take it easy after another intense week of React.  

I decided to branch off on our hackathon project, to fix a screen sizing issue that was occurring on one of my teammates' monitor.  With more freedom on the jsx files, I was able to manage the container layout, and centre everything appropriately, to give  
the header more space to move down (as it was clipping off on their screen). This should fix the issue, but it also made me realise I could add a media query so if the height was below a certain sizing on the viewport, it would disappear, giving the rest of our app  
more breathing space.  
  
After pushing that branch up to the remote repo; I realised I'd like to have those changes myself, so I forked the repo with that unmerged branch.  Which made me realise, I had no idea how to merge it manually, as the github website does not prompt a pull request on a forked repo  
with an unmerged branch. So I had to clone this forked repo, checkout the branch and ensure I had those changes locally, checkout main again, and then use the 'git merge branchname' command, and then push those changes back to the remote repo on main.  

------------ 

--- Day 100 ---  
2025-02-02

Same feeling as yesterday, I'm still winding down from a couple of intense weeks, so using today as a chill winding down coding session.  

I wanted to take the content of my CV (which I've been gradually updating in draft form) and transfer it to a fresh, modern template; therefore I've opened a repo and decided to design my own template.  
Revisiting my basic CSS skills, I managed to create a stylised header, and filled the basic wireframe for each section so far.  

------------ 
