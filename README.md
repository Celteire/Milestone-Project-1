# Milestone Project 1

# Author : Niall Hobson : Created 23/08/2018

# #Project Name : _**Monkees Fan Page**_

This project is all about providing a nostalgic feel good website for the many Monkees fans that grew up ennjoying
their saturday morning crazy romps on television and listening to their numerous hits, including many top ten's and
four number ones.

Although it is not meant to be an exhaustive collection of everything the Monkees did or said which would be for the 
die-hard fans. It is meant to provide a flavour of the Monkees and remind the casual visitor of some happy moments. 
This site also is meant to provide details on what is going on with the Monkees today via the 'blog' and 'hire me' 
sections and also provide links to the super detailed fan sites acccessed through the social links like facebook, 
twitter and youtube.

The four best known songs are linked to a carousel of four pictures new and old of the band. Some of the album covers
are displayed and when clicked on expand, click off they collapse.

In designing this project, I wanted to provide a platform for the user which I envisage will initially want to listen
to the hits !, and then click on the albums before either looking back up to the navigation bar for more information
webpages that appear on the same page or else move down to the footer section where they can subscribe to an email mailing
list for a newsletter and/or choose to open a social media tab to get further information.

The ideas are to provide a user with a hub to get a taster of the 'best of The Monkees' and also to allow the user to get
further details of what is happening now with the Monkees, tours, dates gossip, this can be done through the navigation bar
for internal to the site details and the footer to go to external sources.

Using **Mockplus** to create a template of how the main page and links would look, the mockplus template is in the project files
and called 'Mockplus Project' this file can be opened in the mockplus program.  The file is the wireframe subdirectory.
[link to Mockplus!](https://www.mockplus.com/).

I established from the template the look and feel of the site, where I wanted to put things and the flow.
_________________________________________________________________________________________________________________

## Features

**The Navigation Bar and Header Is Repeated On Every Page**

Starting at the header, the user can see a navigation bar, which allows the user to choose from the following
menu items : *** Home About Us Hire Us Blog Contact ***

### Home Page

Under the navigation bar there is a section with a carousel of four pictures, there are left and right
arrows to move the user between the pictures. There is also a slider bar below the carousel to allow
the user to navigate through the carousel that way or straight to an individual picture. Each picture has
a play / pause button which plays one of the groups four no.1 hits.

_As part of the look and feel, I chose to use the color red for any clickable choices throughout the
system._

Below the carousel section is a link section with just instructions on how to navigate through the next section
I showcased some font-awesome icons.

The next section has a set of six album covers. These pictures are displayed and when clicked expand when clicked
off the screen area of the expanded picture they collapse. You can also click left or right on the expanded
picture to get a carousel effect. I used the external library **ekko-lightbox.js** to achieve this effect.

Finally on the **Home Page** the footer contains the signup for the newsletter and the social links.
The social links when pressed open a new tab and go to the relevant page be it YouTube, Twitter or Facebook.

**The Newsletter and Social Links Are Repeated On Every Page**

_________________________________________________________________________________________________________________

### About Us Page

This page contains the same header and footer as mentioned before. The only content is a horizontal text marquee.
I wanted to use this software feature and originally I had it scrolling as it does when you click on **About Us**
I had an audio autoplay playing the theme song from the Monkees hit TV show from the 70's. However, when I went to test
this feature I found that Google in their wisdom have disabled the autoplay feature in Chrome and although it works on most
other browsers, it seems that unless the user changes settings on their individual chrome installation to allow autoplay, then
there would be no sound. I decided to just wrap the audio behind a simple play / pause button. There was no need to put
in more in this section as the bouncing marquee effect saying you already know about us is tongue in cheek.

_________________________________________________________________________________________________________________

### Hire Us

This page contains the _Hire Us_ and _Frequently Asked Questions_ sections. Both sections are based on the card classes of bootstrap.
The FAQ section also has data toggling for the questions which open and collapse when clicked. It is a Bootstrap defined HTML5 data
attribute. Same header and footer as before.

_________________________________________________________________________________________________________________


### Blog

The Blog page is a simple card class system showing quotes from fans and responses from the extant band members.
Same header and footer.

_________________________________________________________________________________________________________________

### Contact

Using Bootstrap card and form classes to get fan details in the first section. Which would allow fans to send mail and
basically join a mailing list. Followed by showing the band photos in rounded shapes and their birth dates etc. Same header
and footer.

_________________________________________________________________________________________________________________


## Unimplemented Features

1. I would like to have hidden the menu item that is currently active.
2. On mobile to scale the carousel and play button. At this time on Mobile it just has the slider and arrows
   to change the pictures.
3. More sophisticated input validation for the form fields and the email field

## Other Ideas

1. Monetise the site with adwords or similar.
2. Establish Merchandising section and connect credit card and paypal links.

## Technologies Used

1. HTML5
2. CSS3
3. Javascript
4. jQuery
5. Bootstrap
6. Font-Awesome 
7. Ekko-Lightbox - Link above 
8. GitHub
9. NotePad++
10. Cloud9

## Special mention

On the carousel, I wanted to implement an audio feature on a bootstrap styled button control, which would start and stop play.
I spent a considerable amount of time trying dozens of html / css ideas to get it the way I wanted but in the end had to write
a javascript function even though I have never used javascript. 

I used document.getElementById("player") to take in my audio control
I used document.querySelectorAll("#control-btn i") to grab the button and then toggle fa play fa pause
I created and array of the 4 song titles and using IndexOf found the correct element in the array that 
was to be operated on.

Once we get into Javascript in the next module, I hope to acquire a deeper knowledge of the The W3C Document Object Model.

Like with every part of this program, I utilised google and found help in places like slashdot / sourceforge / w3schools / youtube
and many other sites that came up in searches and I found snippets of code here and there which I was sometimes able to modify for
my own use. normally though most samples did not help and 1 in 10 would just point me in the right direction.

### Testing

Throughout development I was calling up google chrome devops to test areas like responsiveness and to try and find out what was wrong when
things were not working. 

I have exporting my code to the W3C markup validation service for testing all my HTML files and tried to fix any anomalies or
syntax or any notified warnings that were reported. [link to html validator!](https://validator.w3.org).

I exported my CSS style sheet to the W3C CSS validation service [link to CSS validator!](https://jigsaw.w3.org/css-validator/).

I also tested the mobile responsiveness of my site with [link to mobile validator!](https://search.google.com/test/mobile-friendly)

With regard to automated testing this is something that I will take on with more experience in the future. For now I did the following
manual testing.

Every clickable menu item, button, arrow and slider is either fixed red or on hover shows red. So the testing of these clicks would activate
the functionality attached. I have clicked on every item and in every possible order and everything seems to be correct.

With the menu it was important to check that the nav options were opening the a page and the correct page when selected in each html file.
As I tended to minimize the header nav and footer sections in the index.html and block copy to the new html file and just change active and
add in the new html filename to each html file, this did not cause any problems on testing.

On the footer I tested the email was validating for the @ sign. I tested the social links open a new tab and go to the correct site.

On the **Hire Us** page I clicked on all the frequently asked questions and checked the contents were correct and each answer was expanding
and collapsing correctly. The _Get It_ service buttons are not hooked to a purchase/payment system but I clicked on them to see they were
passive.

On the **Contact Us** page the form fields and submit button are not connected to a server and therefore are passive, if you enter data in
the email without an @ and hover over it after pressing <return> <tab> or clicking off it. It will show the format required but no error message.

I entered data and also left it blank and got no errors on submitting or clicking off it.

I tested this project on simulated desktop, tablet and mobile devices. On mobile I tested the hamburger menu collapsing and expanding.

One area I would like to address is resizing the carousel images for mobile and the play button. If there is time left to achieve this,
I will do.

Deployment was via git in a terminal using git status, git add ., git commit -m "comment", git push -u origin master (username password)

Then in GitHub going to settings under my project and going to the relevant section to deploy. Once deployed any further commits and
pushes are automatically available on the deployed website link.

There should be no differences now between the deployed version and the development version. However during development when I was using
audio autoplay the deployed version was working fine with autoplay, but my development version was not working under chrome. So as mentioned
above I just wrapped the audio behind a button to get around the problem.

Credits : I would like to thank my mentor for pointing me in the right direction a few times. All the work was done by me, with snippets
I gleaned from various internet sources and modified to my use.

All the text was written by me and is mostly fictitious, this website is just for the purposes of the project and not for general public
consumption. Most of the images and audios were provided in the code institute brief. Any other ones did not seem to have any copyright 
notices and as said this site is not for public consumption.
 
