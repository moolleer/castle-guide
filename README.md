# Castle Guide Skåne

Castle guide Skåne is a site for people who are interested in swedish castles and history in the south part of Sweden. 
The site is intended to target people who wants to visit and learn more about castles. It highlights certain castles around Skåne, and will be useful for people who looking for easy and quick information about wich castles could be worth visiting and where they are located.    

![Responsive Mockup](docs/README-images/am-i-responsive.png)

### [View the live website here](https://moolleer.github.io/castle-guide/)

## Features 

### Design

- The color palette for the website was generated from [My Color](https://mycolor.space/). 

![Color palette](docs/README-images/color-gradient.png)

- I have used the colors #75BA75 and #1E8F83 for the background.
- I wanted a smooth gradient effect for the page, and found how to implement it here [Gradient reference](https://www.w3schools.com/css/css3_gradients.asp)
- A white text color is used to give a nice contrast against the green background. 
- I wanted to have an opaque background behind the text, so the background image could still be used with white text.

### Existing Features

Home page
- In the homepage, when first loaded the user welcomes with a zoom out effect on the background image of a castle. 
- The name and location is also stated in a small colored circle to catch the users attention.

![Home page](docs/README-images/homepage-feature.png)

Header
- A header section with the logo and icon. 
- The header is consistent trough the whole site, with responsive design for different screen sizes.
- Navigation links for each page _Home_ (index.html), _About_ (about.html), _Castles_ (castles.html) and _Sign up_ (sign-up.html).
- A colored border effect for letting the user know wich page its currently on.
- The navigation links also have a colored increased padding when hovered over. 

![Header](docs/README-images/header.png)

About Us
- The about section give the user some short info. 

![About](docs/README-images/aboutpage%20.png)

Castles

The castle page contains:

- An image to give the user a perception about the castle looks.
- A clickable map wich opens up in a new tap to give the user a quick perception of the castles location.
- A short describing text about the castle and its history. 
- A link to the castles website.

Responsive design

- How the castle page looks on devices over 1200px 
![Castles over 1200px](docs/README-images/castles-over-1200px.png)

- How the castle page looks on devices over 992px 
![Castles over 992px](docs/README-images/castles-over-992px.png)

- How the castle page looks on devices over 768px
![Castles over 768px](docs/README-images/castles-over-768px.png)

- How the castle page looks on devices over 600px
![Castles over 600x](docs/README-images/castles-over-600px.png)

- How the castle page looks on devices over 300px

![Castles over 300x](docs/README-images/castles-over-300px.png)

- How the castle page looks on devices under 300px

![Castles under 300x](docs/README-images/castles-under-300px.png)

Sign up
- The page contains a form for the user to fill in if they want to have a newsletter for castles updates.

![Sign up form](docs/README-images/signup-page.png)

- The fields requires input and the email field must have a emailaddress.

![Sign up form email](docs/README-images/signup-email.png)

- The button changes color and to uppercase letters when hovered over.

Footer 
- The footer is consistent trough the whole site, with responsive design for different screen sizes.
- It contains the contact details such as email and phonenumber.
- It also contains the icons and links to social media pages, wich will open in a new tab.

![Footer](docs/README-images/footer.png)

- The icons for the social media links and logo have been taken from [FontAwesome](https://fontawesome.com/)

### Future Features
- Make the images clickable and open up a new page for each castle with more information and history.
- Improve the design for different screen sizes, so the alignment is more an even flow of the content. It works on the most dimensions, but theres more room for improvement.

## Testing
### Manual testing

- Text and email inputs in the sign up form are validated.
- All of the websites pages are fully responsive. This was tested by using Google Developer Tool. 
- The website have been tested and works in different browsers:

  - Google Chrome
 ![Google chrome browser](docs/README-images/test-google-chrome.png)

  - Microsoft Edge
 ![Microsoft Edge browser](docs/README-images/test-microsoft-edge.png)

  - Firefox
 ![Firefox browser](docs/README-images/test-firefox.png)

  - Safari
 ![Safari browser](docs/README-images/test-safari.png)

### Lighthouse

All of the website pages have been tested using Lighthouse Chrome Developer Tool.
Lighthouse score on castle page can be improved on future updates. The lower score is negatively effected by the images width and height values that differ from the source images dimension.

 - Home page

![Lighthouse score home page](docs/README-images/lighthouse-home.png)
 - About page

![Lighthouse score about page](docs/README-images/lighthouse-about.png)
 - Castle page

 ![Lighthouse score castle page](docs/README-images/lighthouse-castles.png)
 - Signup form

 ![Lighthouse score sign up page](docs/README-images/lighthouse-signup.png)
 
### External Links
All external links have been tested and opens in a seperate tab when clicked: 
- Links to social media in the footer
- Links to the castles homepages
- Links to Google Maps location

### Code Validation
##### W3C HTML Validation

- Home page
![Home page HTML validation](docs/README-images/Home-page%20.jpg)
- About page
![About page HTML validation](docs/README-images/About.jpg)
- Castles page
![Castle page HTML validation](docs/README-images/castles.jpg)
- Sign up page
![Castle page HTML validation](docs/README-images/signup.jpg)

All html pages are validated with [W3C HTML validator](https://validator.w3.org/) and come back with no errors or warnings.

##### W3C CSS Validation

- W3C CSS Validator
![CSS validation](docs/README-images/css.jpg)
CSS validated by [CSS validator](https://jigsaw.w3.org/css-validator/) and no error found.

### Bugs and fixes

- Links to the castle website in the media query for (max: width 992px) did not work. This was the only media query I used this positioning to, because I wanted the picture and map to appear left of the text. After some research I figured out it had to do with the z-index of the link thanks to this page on [Stackoverflow](https://stackoverflow.com/questions/16773989/when-div-with-absolute-position-is-added-cannot-click-on-links) 
After I changed it to z-index 2 it worked perfectly.

- After deployment the images did not show on the live website. As it worked in Gitpod I could not understand what was wrong. After some reserach I found this page on [Stackoverflow](https://stackoverflow.com/questions/41468951/images-not-displaying-in-github-pages), and after I removed a forward slash from the start of the filepath the images finally worked.

Unfixed bugs

For screen sizes between 600px-768px the empty space between the bottom and top for the following castles differs. I have tried to solve this by changing paddings, margins, positions with different values on all elements.
I have also had some help from my mentor but the time was limited and we had to move on to other topics in our last mentoring session. This would be something I would improve for future. 

## Deployment

The project has been deployed to GitHub pages taking the following steps:

1) In the Github project repository, click on _Settings_.
2) From the Settings menu, locate _Pages_.
3) Under Branch, select _Main_ branch.
4) Click _Save_, and the page will then automatically refresh with a link to the deployed site.

The live link: https://moolleer.github.io/castle-guide/


## Credits
- To Merve my mentor for the guidance and help.

### Content
- Inspiration from the Love Running projects zoom effect for home page and active class for the navigation links.
- Most of the text and inspiration about the castles are based on information from [Swedish nomad](https://www.swedishnomad.com/sv/skanska-slott/) and [Slottsguiden](https://slottsguiden.info/)

### Media   
The images for the castle and background are from following websites: 
 - [Kulturbilder](https://kulturbilder.wordpress.com/2017/09/27/trollenas-slott-eslov/)
 - [Gylleboannika](https://gylleboannika.se/tag/hovdala-slott/)
 - [Skurup](https://www.skurup.se/svaneholm)
 - [Swedish nomad](https://www.swedishnomad.com/sv/skanska-slott/)
 - [Slottsguiden](https://slottsguiden.info/)



















