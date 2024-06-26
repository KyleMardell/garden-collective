## Testing

Testing in development was done using Google Chrome Developer Tools on a Windows 11 machine. While building the site I used the "inspect" option within Google Chrome to display different device screen sizes. I also tested the site on a 1080p and 4k monitor to check for consistancy accross larger screen sizes. 

The site was deployed to GitHub pages early in development. I used this as a way to check that implemented features were diplayed and functioning correctly when not using my development environment. I would test the deplyed site at the end of every session to ensure it was working as expected through the internet, not just a local server. 

I used the W3 Validator for both the HTML and CSS to check there were no errors on the site.

### Validator

- HTML Testing Using The [W3C Validator](https://validator.w3.org/)
    - [Index Page](https://validator.w3.org/nu/?doc=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2Findex.html)
    - [Calendar Page](https://validator.w3.org/nu/?doc=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2Fcalendar.html)
    - [Gallery Page](https://validator.w3.org/nu/?doc=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2Fgallery.html)
    - [Contact Page](https://validator.w3.org/nu/?doc=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2Fcontact.html)
    - [Confirmation Page](https://validator.w3.org/nu/?doc=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2Fconfirmation.html)
    - [404 Page](https://validator.w3.org/nu/?doc=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2F404.html)

- CSS Testing Using The [Jigsaw Validator](https://jigsaw.w3.org/css-validator/)
    - [Index Page](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2Findex.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)
    - [Calendar Page](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2Fcalendar.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)
    - [Gallery Page](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2Fgallery.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)
    - [Contact Page](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2Fcontact.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)
    - [Confirmation Page](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2Fconfirmation.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)
    - [404 Page](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fkylemardell.github.io%2Fgarden-collective%2F404.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)

### Lighthouse

I tested the website using Google Chromes Lighthouse tool for accessibility, performance, best practices and SEO. All categories recieved high scores across both desktop and mobile testing. When testing on mobile the performance scores dropped slightly as expected due to the use of high quality images, but not enough to noticably affect the user experience. When testing the confirmation page, an accessibility score of 92% was achieved due to the use of a redirection meta tag. Although this reduces the score, I believe the use of a confirmation page and redirect to the home page increases the overall user experience.

#### Desktop Results
- [Index Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/index-lighthouse-desktop.png)
- [Calendar Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/calendar-lighthouse-desktop.png)
- [Gallery Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/gallery-lighthouse-desktop.png)
- [Contact Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/contact-lighthouse-desktop.png)
- [Confirmation Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/confirmation-lighthouse-desktop.png)
    - [Accessibility Score](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/accessibility-lighthouse-desktop.png)
- [404 Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/404-lighthouse-desktop.png)

#### Mobile Results
- [Index Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/index-lighthouse-mobile.png)
- [Calendar Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/calendar-lighthouse-mobile.png)
- [Gallery Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/gallery-lighthouse-mobile.png)
- [Contact Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/contact-lighthouse-mobile.png)
- [Confirmation Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/confirmation-lighthouse-mobile.png)
    - [Accessibility Score](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/accessibility-lighthouse-mobile.png)
- [404 Page](https://github.com/KyleMardell/garden-collective/blob/main/media/lighthouse/404-lighthouse-mobile.png)

### WAVE

All pages of the site were tested using the Web Accessibility Evaluation Tool (WAVE).

The error that is raised on each page is due to using a checkbox input as a dropdown menu. The label contains an icon instead of text and produces an 'Empty form label' warning, This is because i have used only HTML and CSS to create the dropdown menu.

There is an error on the contact page for a 'Missing form label'. The label is present in the HTML for the use of screen readers but hidden using CSS for a cleaner looking form. Here I have used a placeholder containing the words 'Enter your message here' to let the user know where to input their contact message.

On the confirmation page there is an error for 'Page refreshes or redirects' due to using a redirect tag as described in the [lighthouse](#lighthouse) testing.

The alerts on each page are for a 'Redundant link'. This is caused by having all page links in the menu visible on each page for consistancy.

There is an additional alert for 'Possible heading' in the index page within the hero section text box. Here I have used a heading for the club name and paragraph text for the address, the address causing the alert.

- [Index Page](https://github.com/KyleMardell/garden-collective/blob/main/media/wave/index-wave.png)
- [Calendar-Page](https://github.com/KyleMardell/garden-collective/blob/main/media/wave/calendar-wave.png)
- [Gallery Page](https://github.com/KyleMardell/garden-collective/blob/main/media/wave/gallery-wave.png)
- [Contact Page](https://github.com/KyleMardell/garden-collective/blob/main/media/wave/contact-wave.png)
- [Confirmation Page](https://github.com/KyleMardell/garden-collective/blob/main/media/wave/confirmation-wave.png)
- [404 Page](https://github.com/KyleMardell/garden-collective/blob/main/media/wave/404-wave.png)

### User Testing

In the user testing stage I had deployed the site on GitHub Pages and asked friends and course peers to test the site for both functionality and looks. Here is some of the feedback I recieved and what I changed on the site to reflect this feedback.

- Paragraph text did not fit the style of the site and should follow the style of the heading font
    - Changed the font to a more 'handwritten' style to better suit the site
- Signup page form is more of a contact form than a signup form
    - Changed naming of 'Signup' to 'Contact' to better suit
- Desktop headings seems small for the screen size
    - Increased heading sizes in home and calendar pages

### Site Testing

I tested the funtionality of the site on multiple browsers, including Chrome, Firefox, Edge and Safari. 

I tested responsiveness of the site and links using the following physical devices:
- Windows PC
- Apple Macbook Pro (2023)
- iPad pro (2021)
- iPhone 15
- Galaxy S20

Testing included:
- Internal links
    - Tested all links to internal pages work correctly
- External links
    - Tested all external links open in a new browser window 
- Nav bar
    - Tested dropdown works as intended on mobile devices
    - Tested expanded nav bar is shown correctly on larger deviced
- Home page
    - Tested home page is responsive and changed layout per device
- Gallery
    - Tested gallery is resposive and changes layout per device
    - Tested background colour is displayed on large screens due to masonry style layout
- Calendar
    - Tested calendar page is responsive and changes layout per device
- Contact form
    - Tested contact form for warning messages and correct submission
- Images
    - Tested all images are displayed on all devices

#### Manual Testing

| Feature | Expected Outcome | Test Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
| NAVBAR |
| Logo text link | When clicked redirects to the home page | Clicked logo | Redirected to home page | Pass |
| Navbar Home link | When clicked redirects to the home page | Clicked link | Redirected to home page | Pass |
| Navbar Home link: hover (desktop) | Changes colour when hovered over with mouse | Hovered mouse over link | Link changed colour | Pass |
| Navbar Calendar link | When clicked redirects to the home page | Clicked link | Redirected to Calendar page | Pass |
| Navbar Calendar link: hover (desktop) | Changes colour when hovered over with mouse | Hovered mouse over link | Link changed colour | Pass |
| Navbar Gallery link | When clicked redirects to the Gallery page | Clicked link | Redirected to Gallery page | Pass |
| Navbar Gallery link: hover (desktop) | Changes colour when hovered over with mouse | Hovered mouse over link | Link changed colour | Pass |
| Navbar Contact link | When clicked redirects to the Contact page | Clicked link | Redirected to Contact page | Pass |
| Navbar Contact link: hover (desktop) | Changes colour when hovered over with mouse | Hovered mouse over link | Link changed colour | Pass |
| Navbar burger icon (mobile) | Displays dropdown menu | Clicked icon on mobile device | Opened dropdown menu | Pass |
| FOOTER |
| Footer Facebook link | When clicked opens Facebook page in a new tab | Clicked link | Opened Facebook page in a new tab | Pass |
| Footer Facebook link: hover (desktop) | Changes colour when hovered over with mouse | Hovered mouse over link | Link changed colour | Pass |
| Footer X/Twitter link | When clicked opens X/Twitter page in a new tab | Clicked link | Opened X/Twitter page in a new tab | Pass |
| Footer X/Twitter link: hover (desktop) | Changes colour when hovered over with mouse | Hovered mouse over link | Link changed colour | Pass |
| Footer Instagram link | When clicked opens Instagram page in a new tab | Clicked link | Opened Instagram page in a new tab | Pass |
| Footer Instagram link: hover (desktop) | Changes colour when hovered over with mouse | Hovered mouse over link | Link changed colour | Pass |
| INDEX PAGE |
| Info section images (desktop) | Images displayed in addition to text | Displayed on desktop screen compared to mobile | Images displayed | Pass |
| Call to action link | When clicked redirects to the Contact page | Clicked link | Redirected to Contact page | Pass |
| Call to action link: hover (desktop) | Changes colour when hovered over with mouse | Hovered mouse over link | Link changed colour | Pass |
| CONTACT PAGE |
| Form Submit | Error message | Submitted form without first name entered | Error shown: focused on first name text box | Pass |
| Form Submit | Error message | Submitted form without last name entered | Error shown: focused on last name text box | Pass |
| Form Submit | Error message | Submitted form without email address entered | Error shown: focused on email address text box | Pass |
| Form Submit | Error message | Submitted form without message entered | Error shown: focused on message text box | Pass |
| Form Submit | Error message | Submitted form with incorrect email address type | Error shown: focused on email address text box | Pass |
| Form Submit button | When clicked submits form and displays confirmation page | Clicked submit with correct form information | Confirmation page shown | Pass |
| Form Submit button: hover (desktop) | Changes colour when hovered over with mouse | Hovered mouse over button | Button changed colour | Pass |
| Confirmation Page |
| Redirect | Redirects to home page after 10 seconds | Submitted form | Confirmation page displayed and redirected to home page after 10 seconds | Pass |

### Bugs

#### Fixed In Development

- Nav bar text not aligned with logo text
    - Removed padding to correctly align all items is the nav bar
- Hero text not filling container/div
    - Aligned text to center on larger screens
- Info images not resizing to fit design
    - Used a div for consistant sizing and added the image as a background to maintain aspect ratio
- Contact page image not filling the screen
    - I was applying the image to a div instead of the section. Applied image to section background
- Background images on calendar and contact pages exceeded screen height
    - I had set the min 'height' to viewport 'width', changed to viewport height as intended

#### Unfixed Bugs

- User can choose not to select any checkbox on the signup page
    - It is not possible to make at least one checkbox 'required' using only HTML and CSS and requires the use of JavaScript

