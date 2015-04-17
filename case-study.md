# Case Study: Write Songs Template Redesign

The web has changed incredibly in the last five years. I used to work on websites, but, due to some life changes, I haven't been able to keep up on new development practices until recent months. It's amazing how technologies have changed and developed. Sites are now expected to be responsive, HTML5 and CSS3 enable new design capabilities with little or no JavaScript, and Zeldman doesn't talk about web standards much. How about that! 

I started refreshing some of my base knowledge using Treehouse recently, but to really dive in, I needed a project.

## The Project

Write Songs is a template I designed and developed in 2011 for a Tumblr blog I had at the time. While designing it, I kept the focus on typography and layout instead of flashy images and illustrations, which were popular at the time. Readability and simplicity were key goals when originally designing the project.

## Project Goals

I decided to take the Write Songs template and redesign and re-develop it nearly from the ground up. 

Upon reviewing the previous design, three major project goals I landed on were to:
1. Make the site responsive
2. Clean up & modernize the design
3. Continue to focus on content and typography

## Process to Goals

### Fonts
The most important part of this project was choosing fonts. The previous fonts used were fairly basic, but were small and the font pairing of sans serif for headers and serif for body copy frankly didn't look that great. 

I used Google Fonts for high quality, cross-platform available fonts into the design.

I chose Droid Serif for the body font as it is very readable and clean. To add variation, I chose EB Garamond, as it is similar to Droid Sans, but different enough to create visual interest. 

### Elements

I spent some time to take inventory of the current elements of the design. After deliberation, I whittled the list of design elements down to what is needed.

* Logo
* Navbar
* Center aligned blog content (big text, easy to read for longer form)
* Content Types
	* Text
	* Blockquote Post
	* Image Post
	* Video
* Page navigation
* Newsletter Box
* Footer

### Restructuring HTML

The previous site used XHTML standards, divs with classes, and slightly less readable code. I took time to clean up the code and change the HTML standard to HTML5, which afforded the ability to use elements like `<header>` and `<section>` to semantically structure the site. I also kept mobile devices in mind when developing the structure of the site, as I aimed for designing a *mobile-first* site.

### Major Presentation Components

#### Antialiasing

Upon inital use of the selected fonts, aliasing made the copy slightly unreadable. After doing some research, I settled on using CSS anti-aliasing with the below code:

`body {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-shadow: 1px 1px 1px rgba(0,0,0,0.004);
}`

The results were dramatically more readable text and content appearing brighter and appealling.

#### Large, Centered Content

The previous design had a standard two column layout, typical of blogs. However, its content felt constrained and small. To clean up the design and make it feel more modern, I chose to center the content and set the base font size to 1.6em with a line height of 1.6em. 

Content is large, easy to read, and, with the font differentiation between header and body copy, more scannable.

#### Newsletter Box

An important element in marketing today is the email newsletter. As a result, I felt it important to include a newsletter signup box on the page. It is centered at the bottom of the page above the footer, and includes a responsive form.

### Responsiveness

The two major elements which required different styling for varying screen sizes are the header and newsletter box. 

For the header, I floated the logo and navbar to the left and right, respectively. I made the header font sizes larger for bigger screens to maintain appeal and readability.

The newsletter box was an interesting undertaking. At sizes higher than 700px, the form elements were no longer appropriately spaced; therefore, above 700px, I floated the elements to be on the same line. I also made the image and copy for the newsletter into a two column layout at above 940px, improving the readability.

## Conclusion

This was my first foray into hand-coding a responsive page. I'd previously used Twitter Bootstrap and Foundation to do so, so this was definitely a learning experience on how responsive CSS functions.

I also found myself amazed at the power of CSS3 when I discovered CSS-powered anti-aliasing for type. 

Though there is much more for me to discover, this project did exactly what it was meant to: refresh my code knowledge, get my feet wet with new ideas on the web, and re-whet my appetite to code.

