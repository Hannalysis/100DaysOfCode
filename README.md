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
