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
  2024-11-01

  I started the day by seeing if I could tidy up my text output from yesterday's project. After 20 minutes of looking up and trying various methods, I realised I called the variables inside the f string as a key value pairing! 
  Once I separarted the key and value into their own curly brackets, the parentheses were omitted in the text output:

  f"{song, top_one_hundred_songs[song]}\n" **-->** f"{song}, {top_one_hundred_songs[song]}\n"

  I then spent a surprisingly large amount of time trying to install node.js on my windows machine. The environment seemed to only work per launch of powershell, so it took additional research, and guidance from a fellow web dev.
  Managed to get to node and npm version checks to register upon each launch without manual input once a solution was found for the env, so calling that a win for the day.

------------
  
