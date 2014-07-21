#### Include an inline screenshot of your codeschool's points from the profile page:
![Alt text](http://hamberguesa.github.io/week-2/1-Chrome-Dev-Tools/imgs/Code School Screenshot.png)

<!-- Modify the Markdown to include your answers. Don't delete the questions! -->

##QUIZ
* Explain which tabs support the following actions and how.
  * Realtime editing of HTML and CSS 
  * Javascript Debugging
  * Performance Optimization 

Realtime editing of HTML and CSS is supported by the Elements and Sources tabs.  You can edit both the HTML and CSS in Elements by directly typing into the windows, however, the changes are temporary.  In the Source tab, you can edit the sources files by typing directly into the window and can either save to browser storage by command S, or save over the original source file by right clicking > save as > and overwriting the original source file.

Javascript Debugging takes place in the Console tab, working in conjunction with the Source tab.  In the Source tab, there are useful buttons for debugging, including the pause, resume, stepover, step into, step out and deactivate buttons.

Performance Optimization takes place in the PageSpeed tab, interacting with the Network tab and the Source tab.  You run PageSpeed Insights for Chrome in your PageSpeed Tab, which will download the page and run several automated checks against it.  You can use the Google Closure Compiler to minify Javascript files and input the minified file into the source sode.  You can also delete problem files from the source code, list CSS before Javascript in the source file, and add 'async' in the Javascript tag in your HTML code in the source code to put off parsing of Javascript so the webpage can be redered sooner.  The Network tab allows you to access all files loading, obtain resource information (size, type, etc.), obtain server response details, and a timeline of network requests. 

* What's the quick key for your OS to spawn the Dev Tools inspector?

command + option + i

* Go to http://www.postmachina.com/ and analyze and tweak this nicely designed page.
  * What is the current background color for the page?  (Surprisingly, it's not just black!)

  #0b0f11, #afafaf; a combination of black, blue, orange and green depending on where the cursor is. 

  * Tweak the background color to white.


  * Tweak the height of the side bar that contains the logo.  Shrink it down to 85px.

  * Roll over the navigation links.  When you hover over them, they dissapear.  Let's change the hover color to black instead.

  * Now take a screenshot of your new (and maybe not so improved) design.  It should match this screenshot: http://postimg.org/image/5ak1jkpl5/

  * Upload your own image to the imgs directory in the `1_Chrome_Dev_Tools` directory.  It should match the image above. The last nav link in the image above is black because the mouse was hovering there when the screenshot was taken. Do the same, and don't take a screenshot of your whole desktop, just the browser window. (This is part of the challenge.)

* For the postmachina website, why can't you tweak the color of the text "The most important things are not things"?  Please explain.

Beacuse it's an image/.gif

* Go to www.ticketswizard.com and analyze the page.  
  * What is the largest image on the website? 

A picture of times square - 92624182-c482-4a35-8da2-4fbf2f502e94_Large_Large.png


  * Explain how you would find out this information, and list the URL of offending image here and how big it is.

  I went to the network tab, disabled cache, cleared the tab and refreshed the page.  Then I sorted by size and found the largest image: 

  92624182-c482-4a35-8da2-4fbf2f502e94_Large_Large.png

  316 KB



* Test the www.ticketswizard.com website with google's [PageSpeed Insights](http://www.ticketswizard.com/).  (You can also download the chrome plugin).  What is the easiest thing to change to optimize the website?  How many kilobytes of data can be eliminated?

Defer parsing of Javascript; 597.5KiB