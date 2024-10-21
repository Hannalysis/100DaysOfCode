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

 
