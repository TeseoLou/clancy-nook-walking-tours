# **Testing**

Testing is a crucial phase in web development that ensures the functionality, usability, and overall performance of a website. This document covers various aspects of manual testing, including responsiveness, browser compatibility, user stories and features. Automated testing was also used to ensure code quality, with HTML and CSS validators checking adherence to web standards. Website performance and SEO was evaluated, while accessibility testing ensured compliance with standards for an inclusive user experience.

## **Manual Testing**

Manual testing was a critical part of the Clancy Nook Project, ensuring that all features functioned correctly and provided a seamless user experience. Testing was conducted throughout the entire development process, incorporating real-time adjustments and refinements.

A combination of DevTools, BrowserStack, and WAVE was used to conduct thorough testing:

- _DevTools_ allowed for in-depth inspection of responsive design, element behavior, and debugging across multiple screen sizes.

- _BrowserStack_ enabled cross-browser compatibility testing, making it possible to simulate older browser versions and various operating systems.

- Regular deployment through _GitHub_ allowed for frequent testing iterations, making it easier to catch and address issues early in the development process.

### **Responsiveness**

To ensure that the website adapts properly across different screen sizes and devices, manual testing was conducted using available physical devices at the time, including smartphones, tablets, and desktops, as well as _DevTools_ in modern web browsers. 

Developer tools allowed for an extended range of responsiveness testing by simulating multiple screen resolutions beyond the available physical devices. This enabled testing for various breakpoints, ensuring the design adapts well to different viewport sizes, including those not physically available for testing.

The table below presents the results of the responsiveness testing, detailing how the site performs across various devices. Key aspects tested include:

- Layout adjustments for different screen sizes.
- Proper display of images and links.
- Consistency in rendering across different devices.

|Responsiveness          |Galaxy S22|Samsung Galaxy Tab S9 Re|Surface Laptop 4|iPhone 12 Pro|iPad Air|MacBook Air Retina|Desktop 1920x1080|
|------------------------|----------|------------------------|----------------|-------------|--------|------------------|-----------------|
|Site responsive >= 700px|n/a       |✔                       |✔               |n/a          |✔       |✔                 |✔                |
|Site responsive < 699px |✔         |n/a                     |n/a             |✔            |n/a     |n/a               |n/a              |
|Links / URLs work       |✔         |✔                       |✔               |✔            |✔       |✔                 |✔                |
|Images display properly |✔         |✔                       |✔               |✔            |✔       |✔                 |✔                |
|Renders as expected     |✔         |✔                       |✔               |✔            |✔       |✔                 |✔                |

### **Browser Compatibility**

To ensure the website functions and appears consistently across different web browsers, manual and automated testing was conducted. This process involved testing on physical devices, as well as using a trial of _BrowserStack_, a cloud-based testing platform that allows for compatibility testing across a wide range of browsers, including versions not available on local machines.

Using BrowserStack was beneficial for:

- Verifying cross-platform consistency across different operating systems (Windows, macOS, and mobile browsers).
- Identifying rendering inconsistencies that may not appear in a single development environment.

The table below presents the results of the browser compatibility testing, detailing how the core features performed across Chrome, Edge, Firefox, Opera, and Safari.

|Feature        |Chrome        |    |Edge          |      |Firefox       |   |Opera         |     |Safari        |    |
|---------------|--------------|----------|--------------|----------|--------------|----------|--------------|----------|--------------|----------|
|               |**Functionality**|**Appearance**|**Functionality**|**Appearance**|**Functionality**|**Appearance**|**Functionality**|**Appearance**|**Functionality**|**Appearance**|
|Navbar         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Footer         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Hero Banners   |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|About Section  |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Tours Overview |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Booking Guide  |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Tours Sections |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Review Tiles   |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Review Guide   |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Contact Form   |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Gallery Page   |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Success Message|Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |
|Error Message  |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |Good             |Good         |

### **User Stories**

To validate that the website meets user needs, a user stories testing phase was conducted. The user stories which had been addressed and their corresponding acceptance criteria had been developed throughout the project using GitHub's issue tracking system to ensure a structured approach.

For testing, the user stories table was shared with ten individuals who represented a diverse group in terms of computing knowledge. This included users with varying levels of technical proficiency, from casual web users to those with more advanced digital skills.

This approach was crucial for testing because:

- Users with limited technical knowledge helped identify issues with usability and intuitive navigation.
- More users could assess technical aspects such as functionality and efficiency.
- A diverse group provided varied feedback, ensuring the website catered to a broad audience, including tourists, locals, and corporate clients.

Each participant tested the website against the acceptance criteria outlined for each user story. They were asked to:

- Navigate the website as they would if they were genuinely looking to book a tour.
- Check accessibility to ensure that information was easy to find and understand.
- Attempt key actions, such as booking a tour, submitting a contact form, or reading reviews.
- Provide feedback on usability, responsiveness, and whether the acceptance criteria were met.

The results of the user stories testing are documented in the table below, showing whether each story passed or failed based on real user interactions.

|User Story                                                                                                                                 |Priority|Acceptance Criteria                                                                                                                                                                                                                          |Pass or Fail|
|-------------------------------------------------------------------------------------------------------------------------------------------|--------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------|
|_As a tourist, I want the website to be easy to navigate, allowing me to quickly find tour information._                                   |🔴      |The website must feature an intuitive main navigation menu, with clearly labelled links to key sections such as tour themes, schedules, pricing, and contact information.                                                  |✔           |
|                                                                                                                                           |        |Tour details, including descriptions, meeting points, and booking links, should be easy to locate within no more than two clicks from the homepage.                                                                  |✔           |
|                                                                                                                                           |        |The website must be fully responsive, ensuring a seamless and user-friendly experience on desktops, tablets, and mobile devices.                                                                                          |✔           |
|                                                                                                                                           |        |Include a visible feedback form or section where users can share their experience, ask questions, or leave testimonials about their tour.                                                                                |✔           |
|                                                                                                                                           |        |A custom-designed 404 page should guide users back to the main sections of the website if they encounter a broken or incorrect link. This page should maintain the site's branding and provide clear options for navigation.|✔           |
|_As a local, I want to read about the guide’s expertise and background so that I can appreciate the depth of historical knowledge offered._|🔴      |The guide's expertise and background are prominently featured on the site.                                                                                                                                                                   |✔           |
|                                                                                                                                           |        |The content includes an engaging biography with relevant credentials and experience.                                                                                                                                                         |✔           |
|                                                                                                                                           |        |The guide's profile includes a high-quality image.                                                                                                                                                                                           |✔           |
|_As a returning user, I want to find other available tours so that I can book a different tour._                                           |🔴      |A dedicated section on homepage lists all available tours.                                                                                                                                                                                   |✔           |
|                                                                                                                                           |        |Each section links to the tours page.                                                                                                                                                                                                        |✔           |
|                                                                                                                                           |        |Tour Page includes 4 section each focusing on a specific tour.                                                                                                                                                                               |✔           |
|                                                                                                                                           |        |Each tour includes descriptions, image core features and meeting point.                                                                                                                                                                      |✔           |
|                                                                                                                                           |        |Provide a "Contact" button.                                                                                                                                                                                                                  |✔           |
|                                                                                                                                           |        |Section on Tours Page guides customer on how to book.                                                                                                                                                                                        |✔           |
|_As a new user, I want to learn about the tours’ themes and details so that I can decide which tour to book._                              |🔴      |A dedicated "Tours" page provides descriptions of available tour themes.                                                                                                                                                                     |✔           |
|                                                                                                                                           |        |Pricing, distance, duration, meeting points and age requirements are clearly displayed for each tour.                                                                                                                                        |✔           |
|                                                                                                                                           |        |Visuals (e.g., images or icons) accompany the descriptions to enhance user engagement.                                                                                                                                                       |✔           |
|_As a new user, I want clear instructions on how to book tours so that I can easily reserve my spot on a Clancy Nook tour._                |🔴      |A dedicated "How to Book" section provides a step-by-step guide on the tours page.                                                                                                                                                           |✔           |
|                                                                                                                                           |        |A prominent Contact button available on all pages.                                                                                                                                                                                           |✔           |
|                                                                                                                                           |        |A prominent Eventbrite button available on tours page.                                                                                                                                                                                       |✔           |
|_As a new user, I want to know how to contact the tour guide so I can ask questions about the services they offer._                        |🔴      |A "Contact" section or page is clearly accessible from the main navigation menu and footer.                                                                                                                                                  |✔           |
|                                                                                                                                           |        |The "Contact" section provides multiple contact options, including email, phone number, and a contact form.                                                                                                                                  |✔           |
|                                                                                                                                           |        |The contact form is functional, with fields for name, email, subject, and message.                                                                                                                                                           |✔           |
|_As a local, I want to easily contact the tour guide so that I can ask about specific tour routes._                                        |🔴      |A "Contact" section/page is easily accessible via the navigation menu and footer.                                                                                                                                                            |✔           |
|                                                                                                                                           |        |The contact form includes a dropdown or text field specifically for inquiries about tour routes.                                                                                                                                             |✔           |
|                                                                                                                                           |        |Contact details (email and phone) are clearly displayed for direct inquiries.                                                                                                                                                                |✔           |
|_As a returning user, I want to be able to contact the tour guide so I can ask about upcoming tours._                                      |🔴      |A "Contact" section or page is easily accessible from the main navigation menu and footer.                                                                                                                                                   |✔           |
|                                                                                                                                           |        |The Footer provides multiple communication options, such as email, phone.                                                                                                                                                                    |✔           |
|                                                                                                                                           |        |The contact form allows users to specify their inquiry.                                                                                                                                                                                      |✔           |
|_As a local, I want to see reviews from other attendees so that I can feel confident about the tour’s quality._                            |🔴      |A "Reviews" page is prominently displayed on the site.                                                                                                                                                                                       |✔           |
|                                                                                                                                           |        |Reviews include feedback content, and ratings.                                                                                                                                                                                               |✔           |
|                                                                                                                                           |        |The reviews are styled for readability and fit seamlessly with the site’s theme.                                                                                                                                                             |✔           |
|                                                                                                                                           |        |Button is available on Reviews page for viewers to visit TripAdvisor                                                                                                                                                                         |✔           |
|_As a returning user, I want to be able to write a review so I can encourage others to book a tour._                                       |🔴      |A review subject is provided on contact form.                                                                                                                                                                                                |✔           |
|                                                                                                                                           |        |Tripadvisor button is clearly shown on reviews page of website and contact page.                                                                                                                                                             |✔           |
|                                                                                                                                           |        |Guide on how to leave a review is provided at the top of the reviews page.                                                                                                                                                                   |✔           |
|                                                                                                                                           |        |Users can input their name, review, and rating for the tour they attended.                                                                                                                                                                   |✔           |
|                                                                                                                                           |        |Confirmation feedback is shown after successfully submitting a review.                                                                                                                                                                       |✔           |
|_As a new user, I want to view a gallery of images from past tours so that I can get a sense of the experience._                           |🟡      |A visually appealing gallery is available on the website, accessible from the navigation bar or home page.                                                                                                                                   |✔           |
|                                                                                                                                           |        |Each image includes descriptive alt text for accessibility purposes.                                                                                                                                                                         |✔           |
|                                                                                                                                           |        |The gallery is responsive, ensuring a good viewing experience on mobile, tablet, and desktop devices.                                                                                                                                        |✔           |
|_As a tourist, I want to access clear meeting point details so that I can find the starting location easily._                              |🟡      |In each section on the Tours Page, there are clear details about the meeting points for each tour.                                                                                                                                           |✔           |
|_As a corporate user, I want to find information about private tours for businesses so that I can book a group experience._                |🟡      |A dedicated tour card on homepage with link provides user with knowledge that private tours are offered.                                                                                                                                     |✔           |
|                                                                                                                                           |        |A dedicated section on tours page provides details about private tours.                                                                                                                                                                      |✔           |
|                                                                                                                                           |        |Include a contact form or link for inquiries about private bookings.                                                                                                                                                                         |✔           |
|_As a returning user, I want to be able to send images to the tour guide so that I can share my experience._                               |🟡      |The file upload field accepts only image file types (e.g., .jpg, .png).                                                                                                                                                                      |✔           |
|_As a returning user, I want to find social media links in the footer so that I can follow updates and share my experience._               |🟡      |Social media icons (e.g., Instagram, Facebook, and Twitter) are prominently displayed in the footer.                                                                                                                                         |✔           |
|                                                                                                                                           |        |Each icon is clickable and links to the relevant Clancy Nook social media pages, opening in a new tab.                                                                                                                                       |✔           |
|                                                                                                                                           |        |A call-to-action message encourages users to follow and share their experiences, such as "Follow us for updates and share your stories!"                                                                                                     |✔           |

### **Features Testing**

Due to the scale of the website and the number of interactive elements, feature testing was conducted manually, primarily by myself. This allowed for a thorough and detailed review of each component, ensuring functionality, responsiveness, and consistency.

To perform this testing, I:

- Manually navigated the website across different pages, testing all interactive elements.
- Resized the browser window to check responsiveness and layout adjustments.
- Interacted with forms, buttons, and hover effects to ensure expected behavior.
- Verified links and redirections to ensure all navigation elements function correctly.
- Checked animations and hover effects to confirm smooth and visually consistent interactions.

The following table summarizes the expected outcomes, testing performed, and results for each feature tested on the website.

|Feature        |Expected Outcomes                                                                                                   |Testing Performed                                                           |Result                                                                                    |Pass/Fail|
|---------------|--------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|------------------------------------------------------------------------------------------|---------|
|Navbar         |Should be sticky and always visible when scrolling.                                                                 |Scrolled up and down the page to verify.                                    |Navbar is sticky and visible while scrolling.                                             |✔        |
|               |Should collapse into a hamburger menu on small screens.                                                             |Resized browser and tested mobile view.                                     |Navbar collapses into hamburger icon on mobile and tablet devices.                        |✔        |
|               |Home button should navigate to the homepage.                                                                        |Clicked on "Home"                                                           |Home button navigates to home page from all pages.                                        |✔        |
|               |About button should navigate to the about section.                                                                  |Clicked on "About"                                                          |About button navigates to about section on  homepage from all pages                       |✔        |
|               |Tours button should navigate to the tours section.                                                                  |Clicked on "Tours"                                                          |Tours button navigates to Tours page from all pages                                       |✔        |
|               |Gallery button should navigate to the gallery section.                                                              |Clicked on "Gallery"                                                        |Gallery button navigates to Gallery page from all pages                                   |✔        |
|               |Reviews button should navigate to the reviews section.                                                              |Clicked on "Reviews"                                                        |Gallery button navigates to Gallery page from all pages                                   |✔        |
|               |Contact button should navigate to the contact section/page.                                                         |Clicked on "Contact" and ensured correct navigation.                        |Contact button navigates to Contact page from all pages                                   |✔        |
|               |Contact button should change color on hover.                                                                        |Hovered over the contact button to check color change.                      |Button changes color on hover                                                             |✔        |
|               |Logo should change color on hover.                                                                                  |Hovered over the logo to check hover effect.                                |Logo changes color on hover to a light blue                                               |✔        |
|               |Other navigation links should underline on hover.                                                                   |Hovered over all menu items to check underline effect.                      |Navigation menu items are underlined when mouse hovers over them.                         |✔        |
|Footer         |Instagram link should navigate to the Instagram page in a new window.                                               |Clicked Instagram link and checked redirection.                             |The Instagram link opens in a new tab and directs users to the correct page.              |✔        |
|               |Facebook link should navigate to the Facebook page in a new window.                                                 |Clicked Facebook link and checked redirection.                              |The Facebook link opens in a new tab and directs users to the correct page.               |✔        |
|               |LinkedIn link should navigate to the LinkedIn page in a new window.                                                 |Clicked LinkedIn link and checked redirection.                              |The LinkedIn link opens in a new tab and directs users to the correct page.               |✔        |
|               |Should remain at the bottom of the page.                                                                            |Checked on various screen sizes.                                            |The footer remains anchored at the bottom of the page across all screen sizes.            |✔        |
|               |Mini navbar should move to the side on larger screens.                                                              |Resized browser to ensure correct positioning.                              |The mini navbar shifts to the side as expected on larger screens.                         |✔        |
|               |Home icon in the mini navbar should navigate to homepage and should expand when hovered over.                       |Clicked on "Home" icon check redirection and animation.                     |The home icon expands on hover and correctly redirects to the homepage.                   |✔        |
|               |About icon in the mini navbar should navigate to about section and should expand when hovered over.                 |Clicked on "About" icon, check redirection and animation.                   |The about icon expands on hover and correctly redirects to the about section.             |✔        |
|               |Tours icon in the mini navbar should navigate to tours section and should expand when hovered over.                 |Clicked on "Tours" icon check redirection and animation.                    |The tours icon expands on hover and correctly redirects to the tours section.             |✔        |
|               |Gallery icon in the mini navbar should navigate to gallery section and should expand when hovered over.             |Clicked on "Gallery" icon check redirection and animation.                  |The gallery icon expands on hover and correctly redirects to the gallery section.         |✔        |
|               |Reviews icon in the mini navbar should navigate to reviews section and should expand when hovered over.             |Clicked on "Reviews" icon check redirection and animation.                  |The reviews icon expands on hover and correctly redirects to the reviews section.         |✔        |
|               |Contact icon in the mini navbar should navigate to contact page.                                                    |Clicked on "Contact" icon check redirection and animation.                  |The contact icon expands on hover and correctly redirects to the contact page.            |✔        |
|Hero banners   |Should display a high-quality background image.                                                                     |Verified image loads correctly.                                             |The background image is clear, high-resolution, and loads without issues.                 |✔        |
|               |Should include a call-to-action button.                                                                             |Clicked CTA button to confirm functionality.                                |The CTA button is clickable and correctly redirects users to the intended action.         |✔        |
|               |Should be responsive and scale properly.                                                                            |Tested on different screen sizes.                                           |The hero section scales properly across different devices without distortion.             |✔        |
|               |Text should get larger as screen size increases.                                                                    |Resized window and checked text scaling.                                    |The text adjusts, increasing in size as the screen gets larger.                           |✔        |
|               |Photograph should expand to full width of the screen.                                                               |Ensured image stretches to full width.                                      |The image expands correctly to fill the entire width of the screen.                       |✔        |
|About section  |Should display in a vertically stacked layout on smaller screens.                                                   |Checked mobile view to ensure text appears below the image.                 |On mobile, the section correctly displays in a single-column format.                      |✔        |
|               |Should transition to a two-column layout on larger screens.                                                         |Resized window to ensure correct layout shift.                              |The section smoothly adjusts to a two-column layout on larger screens.                    |✔        |
|               |On larger screens, the photo should be on the left and the title, description, and signature should be on the right.|Ensured proper positioning of elements in desktop view.                     |The layout correctly places the image on the left and text content on the right.          |✔        |
|Tours overview |Should list all available tours.                                                                                    |Verified all tours are listed correctly.                                    |All available tours are displayed clearly with relevant details.                          |✔        |
|               |Cards should be stacked vertically on mobile, in two columns on tablets, and four on laptops.                       |Resized window to verify responsive behavior.                               |The tour cards adjust layout dynamically based on screen size.                            |✔        |
|               |On hover, the shadow should get bigger to enhance interactivity.                                                    |Hovered over the cards and checked for shadow enlargement.                  |The shadow effect increases on hover, enhancing user engagement.                          |✔        |
|               |On hover, the card should expand slightly for a subtle zoom effect.                                                 |Hovered over the card to verify expansion.                                  |Cards slightly expand on hover, providing a visual cue for interactivity.                 |✔        |
|               |On click, users should be taken to the A Tale of Two Cities section on the tours page.                              |Clicked on this tour card and verified redirection.                         |Clicking the card correctly navigates to the A Tale of Two Cities tour section.           |✔        |
|               |On click, users should be taken to the True Crime in Ancoats section on the tours page.                             |Clicked on this tour card and verified redirection.                         |Clicking the card correctly navigates to the True Crime in Ancoats tour section.          |✔        |
|               |On click, users should be taken to the Stories of Whalley Range section on the tours page.                          |Clicked on this tour card and verified redirection.                         |Clicking the card correctly navigates to the Stories of Whalley Range tour section.       |✔        |
|               |On click, users should be taken to the Private Bookings section on the tours page.                                  |Clicked on this tour card and verified redirection.                         |Clicking the card correctly navigates to the Private Bookings section.                    |✔        |
|Booking guide  |Should provide step-by-step instructions.                                                                           |Read through guide to ensure clarity.                                       |The booking guide clearly outlines all necessary steps in a user-friendly format.         |✔        |
|               |Elements should be stacked vertically on smaller screens.                                                           |Checked mobile layout to ensure vertical stacking.                          |The elements display in a single-column layout on mobile for easy reading.                |✔        |
|               |Layout should transition to two columns on larger screens.                                                          |Resized browser to verify proper layout shift.                              |The layout adjusts to two columns on larger screens for improved usability.               |✔        |
|               |Contact button should change color on hover.                                                                        |Hovered over the contact button to check color change.                      |The contact button visually responds by changing color when hovered.                      |✔        |
|               |Eventbrite logo should change color on hover.                                                                       |Hovered over the Eventbrite logo to check color change.                     |The Eventbrite logo color shifts on hover, enhancing user interaction.                    |✔        |
|               |Contact button should navigate users to the contact page.                                                           |Clicked on the button to confirm redirection.                               |Clicking the contact button successfully redirects users to the contact page.             |✔        |
|               |Eventbrite logo should open the Clancy Nook Eventbrite page in a new tab.                                           |Clicked on logo to verify correct link behavior.                            |The Eventbrite logo correctly opens the Clancy Nook Eventbrite page in a new tab.         |✔        |
|Tours sections |Should display images, descriptions, and pricing.                                                                   |Checked images and text formatting.                                         |Each tour card correctly displays an image, details, and a brief description.             |✔        |
|               |Layout should be stacked vertically on smaller screens.                                                             |Checked mobile layout to ensure vertical stacking.                          |Tours are displayed in a single column on mobile for easy readability.                    |✔        |
|               |On larger screens, images should be on one side and title, description, and tour details should be on the other.    |Resized window to confirm correct layout shift.                             |The layout shifts to two columns, ensuring images and descriptions are well-placed.       |✔        |
|               |A Tale of Two Cities carousel should be active by default.                                                          |Loaded the page and checked if the carousel was transitioning automatically.|The carousel automatically rotates through images, showcasing the tour highlights.        |✔        |
|               |A Tale of Two Cities carousel should be controllable with "previous" and "next" buttons.                            |Clicked "prev" and "next" buttons to verify manual control.                 |Users can navigate through images using the previous and next buttons.                    |✔        |
|               |True Crime in Ancoats carousel should be active by default.                                                         |Loaded the page and checked if the carousel was transitioning automatically.|The carousel cycles through tour-related images without user interaction.                 |✔        |
|               |True Crime in Ancoats carousel should be controllable with "previous" and "next" buttons.                           |Clicked "prev" and "next" buttons to verify manual control.                 |The navigation buttons allow users to scroll through images manually.                     |✔        |
|               |Stories of Whalley Range carousel should be active by default.                                                      |Loaded the page and checked if the carousel was transitioning automatically.|The carousel continuously rotates between images of this tour.                            |✔        |
|               |Stories of Whalley Range carousel should be controllable with "previous" and "next" buttons.                        |Clicked "prev" and "next" buttons to verify manual control.                 |Users can switch between images using navigation controls.                                |✔        |
|               |Private Bookings carousel should be active by default.                                                              |Loaded the page and checked if the carousel was transitioning automatically.|The private bookings section displays a rotating gallery of images.                       |✔        |
|               |Private Bookings carousel should be controllable with "previous" and "next" buttons.                                |Clicked "prev" and "next" buttons to verify manual control.                 |Users can manually navigate through the private bookings images.                          |✔        |
|               |Contact button for Private Bookings should change color on hover.                                                   |Hovered over the contact button and verified color change.                  |The button changes color on hover, indicating interactivity.                              |✔        |
|               |Contact button for Private Bookings should direct users to the contact page.                                        |Clicked on the contact button and verified redirection.                     |Clicking the button correctly redirects users to the contact page.                        |✔        |
|Review tiles   |Should be displayed stacked vertically on mobile screens.                                                           |Checked mobile layout to ensure tiles appear in a single column.            |Reviews are listed in a single column on mobile for easy scrolling.                       |✔        |
|               |Should transition to a two-column layout on tablets.                                                                |Resized window to verify tiles display in two columns.                      |The reviews adjust into two columns on tablets for better spacing.                        |✔        |
|               |Should transition to a three-column layout on laptops and larger screens.                                           |Resized window to ensure tiles adapt to three columns.                      |Reviews are displayed in a well-spaced three-column grid on larger screens.               |✔        |
|               |On hover, the tile should slightly expand for a subtle zoom effect.                                                 |Hovered over tiles and verified expansion.                                  |The review tiles slightly expand on hover, enhancing user engagement.                     |✔        |
|               |On hover, the shadow should get bigger for added interactivity.                                                     |Hovered over tiles and checked shadow enlargement.                          |The tile's shadow enlarges on hover, adding a visual effect.                              |✔        |
|               |On hover, the text should get bigger to enhance readability.                                                        |Hovered over tiles and confirmed text size increase.                        |The text enlarges on hover, making it easier to read.                                     |✔        |
|Review guide   |Should display elements stacked vertically on mobile screens.                                                       |Checked mobile layout to ensure proper stacking.                            |Review guidance elements are stacked vertically on mobile for clarity.                    |✔        |
|               |Should transition to a two-column layout on tablets and larger screens.                                             |Resized window to confirm proper layout shift.                              |On larger screens, elements are displayed in two columns for better readability.          |✔        |
|               |On larger screens, TripAdvisor logo should be on one side and title with call-to-action on the other.               |Ensured correct positioning of elements.                                    |The TripAdvisor logo and review section are correctly arranged in two columns.            |✔        |
|               |Contact button should be in the middle at the bottom.                                                               |Verified contact button placement.                                          |The contact button appears centered below the call-to-action section.                     |✔        |
|               |Contact button should take users to the contact page.                                                               |Clicked on the contact button and verified redirection.                     |Clicking the button redirects users to the contact page successfully.                     |✔        |
|               |Contact button should change color on hover.                                                                        |Hovered over the contact button and confirmed color change.                 |The button changes color when hovered, confirming interactivity.                          |✔        |
|               |TripAdvisor logo should change size when hovered.                                                                   |Hovered over the logo and verified size change.                             |The TripAdvisor logo enlarges on hover, making it visually distinct.                      |✔        |
|               |TripAdvisor logo should open Clancy Nook TripAdvisor page in a new tab when clicked.                                |Clicked on logo to confirm correct redirection.                             |Clicking the logo correctly opens the Clancy Nook TripAdvisor page in a new tab.          |✔        |
|Contact Form   |Forename field should require alphabetic input and not be empty.                                                    |Entered valid and invalid names to verify validation.                       |The field accepts alphabetic input only and displays an error for empty or invalid values.|✔        |
|               |Surname field should require alphabetic input and not be empty.                                                     |Entered valid and invalid surnames to verify validation.                    |The field correctly validates alphabetic input and prompts an error for invalid entries.  |✔        |
|               |Email field should require a valid email format.                                                                    |Entered valid and invalid emails to verify validation.                      |The form allows only properly formatted email addresses and shows an error otherwise.     |✔        |
|               |Message subject field should be required.                                                                           |Attempted submission without selecting a subject.                           |The form prevents submission and highlights the missing subject field.                    |✔        |
|               |Message field should be required.                                                                                   |Attempted submission without entering a message.                            |The form prevents submission and highlights the missing message field.                    |✔        |
|               |Phone number field should allow numeric input only and be optional.                                                 |Entered numbers and non-numeric characters to test.                         |The field only allows numeric input and displays an error for non-numeric characters.     |✔        |
|               |Tour selection radio buttons should appear conditionally based on the selected message subject.                     |Selected different subjects to check conditional display.                   |The tour selection buttons appear only when applicable message subjects are chosen.       |✔        |
|               |Tour selection radio buttons should become required when visible.                                                   |Attempted submission without selecting a tour when required.                |The form prevents submission if a tour is not selected when the section is displayed.     |✔        |
|               |Star slider should appear conditionally based on the selected message subject.                                      |Selected subjects related to feedback to check visibility.                  |The star slider becomes visible only when relevant subjects are selected.                 |✔        |
|               |Star slider should become required when visible.                                                                    |Attempted submission without using the slider when required.                |The form prevents submission if the slider is not used when the section is displayed.     |✔        |
|               |Image upload option should appear conditionally based on the selected message subject.                              |Selected subjects related to file uploads.                                  |The image upload feature appears when the selected subject requires image submission.     |✔        |
|               |Image upload should become required when visible.                                                                   |Attempted submission without uploading an image when required.              |The form prevents submission if an image is not uploaded when the section is displayed.   |✔        |
|               |Submit button should change color on hover.                                                                         |Hovered over the submit button.                                             |The button changes color on hover, indicating interactivity.                              |✔        |
|               |Submit button should take users to the success page upon valid form completion.                                     |Submitted form with all required fields filled correctly.                   |The form redirects users to the success page when completed correctly.                    |✔        |
|Gallery        |Images should be stacked vertically on mobile.                                                                      |Viewed gallery on a mobile device.                                          |Images appear in a single-column layout for better visibility.                            |✔        |
|               |Gallery should display a mix of horizontal and vertical images.                                                     |Checked various images displayed.                                           |The gallery includes a variety of horizontal and vertical images.                         |✔        |
|               |Images should be arranged in two columns on tablets.                                                                |Resized browser to tablet dimensions.                                       |The images are displayed in two columns on tablet-sized screens.                          |✔        |
|               |Images should be arranged in three columns on laptops.                                                              |Resized browser to laptop dimensions.                                       |The gallery shifts to a three-column layout for larger screens.                           |✔        |
|               |There should be no gaps between photos.                                                                             |Inspected image spacing.                                                    |Images are arranged seamlessly with no noticeable gaps.                                   |✔        |
|               |On larger screens, the gallery should not stretch the full width of the screen.                                     |Viewed gallery on large screens.                                            |The gallery maintains a centered layout, not stretching to full screen width.             |✔        |
|Success Message|Should display a confirmation message upon successful form submission.                                              |Submitted a valid form and checked the success page.                        |The success message appears immediately after form submission.                            |✔        |
|               |Elements should be stacked vertically on mobile.                                                                    |Viewed success page on a mobile device.                                     |The success message, image, and button are stacked in a single-column format.             |✔        |
|               |Layout should transition to two columns on tablets and larger screens.                                              |Resized browser to tablet and desktop sizes.                                |The success page correctly adjusts to a two-column layout for better readability.         |✔        |
|               |The Clancy Nook image should be interactive and change on hover.                                                    |Hovered over the Clancy Nook image.                                         |The image reacts to hover input, enhancing user engagement.                               |✔        |
|               |The home button should change color on hover.                                                                       |Hovered over the home button.                                               |The button changes color on hover, indicating interactivity.                              |✔        |
|               |Clicking the home button should navigate users back to the homepage.                                                |Clicked on the home button.                                                 |The button successfully redirects users to the homepage.                                  |✔        |
|404 Error Page |Page should only be displayed when a broken link or incorrect URL is accessed.                                      |Entered a broken or incorrect link.                                         |The 404 page only appears when an invalid URL is entered, confirming expected behavior.   |✔        |
|               |Elements should be stacked vertically on mobile.                                                                    |Viewed error page on a mobile device.                                       |The error message, image, and navigation options are displayed in a single-column format. |✔        |
|               |Layout should transition to two columns on tablets and larger screens.                                              |Resized browser to tablet and desktop sizes.                                |The error page adjusts to a two-column layout for improved readability.                   |✔        |
|               |The 404 image should be interactive and change on hover.                                                            |Hovered over the 404 image.                                                 |The illustration reacts to hover input, adding an engaging visual effect.                 |✔        |
|               |The home button should change color on hover.                                                                       |Hovered over the home button.                                               |The button changes color on hover, indicating interactivity.                              |✔        |
|               |Clicking the home button should navigate users back to the homepage.                                                |Clicked on the home button.                                                 |The button successfully redirects users to the homepage.                                  |✔        |

## **Automated Testing**

### **HTML Validation**

To ensure the accuracy and compliance of the HTML code across the deployed website, the _World Wide Web Consortium_ (W3C) Nu HTML Checker was utilized as the primary validation tool. Each page’s HTML code was rigorously tested multiple times through the validator, which proved invaluable during the testing phase.

The primary issues flagged by the validator were:

1. Use of px in the width and height attributes on images – These were removed to ensure a more flexible and accessible design.
2. Incorrect closing tags – Some elements had been improperly closed, which had gone unnoticed when manually reviewing the code for semantic accuracy. For instance, a section element had mistakenly been closed with a div, leading to structural inconsistencies.
3. Misuse of alt text and descriptions – alt attributes had been applied to elements where they were not valid, such as anchor tags. These unnecessary attributes were removed to maintain proper HTML syntax.

After identifying and addressing all issues flagged by the validator, all pages successfully passed the validation process, ensuring the HTML was both structurally sound and standards-compliant.

### **CSS Validation**

To ensure the stylesheets adhered to web standards and best practices, the _World Wide Web Consortium_ (W3C) CSS Validator was utilized. The stylesheet was put through the validation process and successfully passed at CSS Level 3 + SVG, confirming its compliance with modern CSS specifications.

While the validation process did not identify any errors, several warnings were flagged. These warnings are informational and highlight aspects of the stylesheet that may require consideration.

1. URI: TextArea
    - This message typically appears when using the direct input or file upload mode in the validator. It does not indicate an actual problem with the stylesheet but rather a technical limitation of the validation tool.
2. Imported style sheets are not checked in direct input and file upload modes
    - When stylesheets import other CSS files using @import, the validator does not check the contents of those imported styles if the file was uploaded directly or pasted into the validator. This means external styles may not be fully analyzed in this mode.
3. Due to their dynamic nature, CSS variables are currently not statically checked (Warnings at lines: 17, 27, 75, 97, 258)
    - CSS variables (--custom-property) allow for dynamic styling changes, but since their values are determined at runtime, the validator cannot verify their correctness statically. This is a known limitation of CSS validation tools, rather than an issue with the stylesheet itself.
4. Vendor extensions and pseudo-elements (Warnings at lines: 561, 562, 574, 575, 584)
    - -webkit-appearance and -moz-appearance are browser-specific properties used to control the default styling of form elements. They are supported by specific browsers (WebKit for Chrome/Safari and Mozilla for Firefox) but are not part of the official CSS standard. These were necessary for cross-browser compatibility but were flagged as warnings since they are not part of the standard CSS specification.

Despite these warnings, they do not impact the validity of the CSS.

### **Lighthouse Auditing**

To ensure optimal performance, accessibility, adherence to best practices, and SEO compliance, all webpages were thoroughly analyzed using Google Lighthouse. This auditing tool was run in both mobile and desktop modes to evaluate how the website performs across different devices and environments.

#### **Performance**

#### Homepage

The homepage achieved an impressive 97% performance rating in the Lighthouse audit for desktop, demonstrating strong optimization and fast loading times.  When tested on mobile, the performance score was slightly lower at 84%. The reduction in performance was primarily due to the increased load times and resource constraints on mobile devices. 

Despite these high score, several diagnostics were flagged:

1. Preconnect to Required Origins
   - Lighthouse recommended using pre-connect or dns-prefetch to establish early connections to third-party origins, particularly Google Fonts.  
   - While I understood the recommendation, I wasn’t entirely sure how to correctly implement pre-connect confidently.  
2. Largest Contentful Paint (LCP)
   - The Largest Contentful Paint metric identified that the hero image inside #homepage-hero was the slowest-loading visible element.  
   - I attempted some optimizations, but since the image is a crucial part of the design, I wasn’t sure how to further reduce its loading time without sacrificing quality. Preloading the image was suggested, but I was unfamiliar with the correct implementation.  
3. Eliminate Render-Blocking Resources
   - The audit flagged Bootstrap CSS (from JSDelivr CDN) and Google Fonts as render-blocking resources, meaning they delayed the first paint of the page.  
   - Both Bootstrap and Google Fonts were essential for the design and typography of the site. Removing or deferring them would break the layout, and I wasn’t confident in alternatives that wouldn’t compromise the design.  
4. Reduce Unused CSS
   - Some unused CSS rules, particularly from Bootstrap and FontAwesome, were detected in the audit.  
   - Since Bootstrap provides essential styling across the site, I couldn’t remove it entirely. I wasn’t sure how to properly remove unused CSS rules without breaking functionality.  
5. Preload Largest Contentful Paint Image
   - Lighthouse suggested preloading the hero image to reduce its rendering time.  
   - While I understood the concept, I wasn’t sure how to implement it properly.  
6. Image Elements Do Not Have Explicit width and height Attributes  
   - Some images lacked explicit dimensions. 
   - While I tried adding width and height attributes, I wanted the height and width to adjust responsively so only min-height and min-width were applied.  
7. Minify CSS
   - The audit suggested minifying the main stylesheet to reduce its size.  
   - While I knew CSS minification was possible, I wasn’t sure how to properly integrate it into my workflow.  
8. Serve Static Assets with an Efficient Cache Policy  
   - Some images lacked long-term caching policies, meaning they were reloaded more frequently than necessary.  
   - Since the site is hosted using GitHub Pages, I didn’t have full control over caching policies, and I wasn’t sure how to override them effectively.  

#### Tours Page

The Tours Page achieved an exceptional 99% performance rating on desktop, indicating that it is highly optimized for speed and efficiency. The mobile performance score was lower at 76%, reflecting the additional challenges mobile devices face with resource loading, network constraints, and rendering performance. 

Despite these high score, several diagnostics were flagged:

1. Eliminate Render-Blocking Resources
    - The audit flagged Bootstrap CSS (from JSDelivr CDN) and Google Fonts as render-blocking resources, delaying the first paint of the page.
    - Bootstrap and Google Fonts were integral to the design and removing them would compromise the site's appearance and functionality. 
2. Preload Largest Contentful Paint Image
    - The hero image in the #tours-hero section was identified as the Largest Contentful Paint (LCP) element, meaning it took the longest to load. Lighthouse suggested preloading this image to improve page speed.
   - I attempted some optimizations, but since the image is a crucial part of the design, I wasn’t sure how to further reduce its loading time without sacrificing quality. Preloading the image was suggested, but I was unfamiliar with the correct implementation.  
3. Image Elements Do Not Have Explicit width and height Attributes
    - Some images on the page did not have explicit width and height attributes, causing Cumulative Layout Shift (CLS).
    - While I attempted to define static dimensions where possible, some images are dynamically resized, making it difficult to apply fixed values across all screen sizes.
4. Minify CSS
    - The style.css file was flagged for potential minification to reduce its size and improve performance.
    - I wasn't sure how to automate the process effectively within my development workflow.
5. Serve Static Assets with an Efficient Cache Policy
    - The audit detected 20 resources that lacked an efficient caching policy, meaning browsers were forced to re-download assets unnecessarily.
    - Since the site is hosted on GitHub Pages, I had limited control over server caching settings, making this issue difficult to address.
6. Reduce Unused CSS
    - Unused CSS rules were detected in Bootstrap and FontAwesome, adding unnecessary bulk to the stylesheets.
    - Since Bootstrap is a core part of the site's styling, I couldn’t selectively remove unused CSS without risking layout issues. I lacked the expertise to properly tree-shake unused styles.

#### Gallery Page

The Gallery Page performed exceptionally well, scoring 99% in performance on desktop, indicating excellent speed and optimization. The mobile performance score was slightly lower at 85%, primarily due to image-heavy content, render-blocking resources, and caching inefficiencies.

Despite these high score, several diagnostics were flagged:

1. Largest Contentful Paint (LCP)
    - The largest visible element on the page was an image that took 4.18 seconds to fully load. This delay was caused by server response time (TTFB), loading delay, and image rendering time.
    - I attempted some optimizations, but since the image is a crucial part of the design, I wasn’t sure how to further reduce its loading time without sacrificing quality. Preloading the image was suggested, but I was unfamiliar with the correct implementation.  
2. Eliminate Render-Blocking Resources
    - Render-blocking resources included Bootstrap CSS (from JSDelivr CDN) and Google Fonts, which slowed down the initial page rendering.
    - Bootstrap and Google Fonts were essential to the styling and typography of the site. I wasn’t confident in removing or deferring them without breaking the page design.
3. Reduce Unused CSS
    - Unused CSS was detected in Bootstrap and FontAwesome, increasing the overall CSS file size.
    - Since Bootstrap provides the core layout of the site, I couldn’t selectively remove unused styles without risking layout and design issues. 
4. Image Elements Do Not Have Explicit width and height Attributes
    - Some images lacked explicit dimensions, which contributed to Cumulative Layout Shift (CLS).
    - Since many images are dynamically sized, I wasn’t sure how to set fixed width and height values without causing display issues on different devices.
5. Minify CSS
    - The main style.css file was flagged for minification to reduce its size and improve load time.
    - While I knew that minifying CSS is beneficial, I wasn’t sure how to integrate it into my workflow.
6. Serve Static Assets with an Efficient Cache Policy
    - Some images lacked long-term caching, meaning users’ browsers had to re-download them instead of retrieving cached versions.
    - Since the site is hosted on GitHub Pages, I had limited control over cache expiration settings, making this difficult to address.

#### Reviews Page

The Reviews Page achieved a 97% performance rating on desktop, demonstrating strong optimization. The mobile performance was lower at 75%, due to slow rendering times, large background images, and render-blocking resources.

Despite these high score, several diagnostics were flagged:

1. Largest Contentful Paint (LCP)
    - The LCP element was the #reviews-page-background div, which took over 7 seconds to render, due to a large background image, server response delay, and slow rendering time.
    - I altered my CCS to include two photos for my background image, one for desktop and one for mobile however this was still flagged.
2. Eliminate Render-Blocking Resources
    - Bootstrap CSS (from JSDelivr CDN) and Google Fonts were flagged as render-blocking resources, delaying the first paint of the page.
    - Both Bootstrap and Google Fonts were essential to the design and layout of the site. I didn’t know how to defer them without breaking styling.
3. Reduce Unused CSS
    - Unused CSS from Bootstrap and FontAwesome was detected, increasing the total size of the stylesheet.
    - Since Bootstrap is required for styling, I wasn’t confident in removing unused styles without causing unintended layout issues.
4. Preload Largest Contentful Paint Image
    - The audit suggested preloading the large background image (reviews-page-background-image.webp) to reduce loading time.
    - I wasn’t sure how to properly implement preloading for a background image without affecting its styling or positioning.
5. Image Elements Do Not Have Explicit width and height Attributes
    - Some images lacked explicit dimensions, which contributed to Cumulative Layout Shift (CLS).
    - Some images were dynamically loaded, making it difficult to set fixed width and height values across all screen sizes.
6. Minify CSS
    - The style.css file was flagged for minification to reduce its size and improve load time.
    - While I knew that minifying CSS is a best practice, I wasn’t sure how to automate the process effectively.
7. Serve Static Assets with an Efficient Cache Policy
    - Some images lacked efficient caching, meaning they were re-downloaded unnecessarily instead of being retrieved from the browser’s cache.
    - The site is hosted on GitHub Pages, where I have limited control over cache expiration settings, making this difficult to fix.

#### Contact Page

The Contact Page achieved a 97% performance rating on desktop, indicating strong optimization. Additionally, the mobile performance score was 91%, making it the highest-scoring page for mobile performance.

Despite these high score, several diagnostics were flagged:

1. Pre-connect to Required Origins
    - The audit suggested adding pre-connect or dns-prefetch for Google Fonts and FontAwesome, which would reduce latency by pre-establishing early connections.
   - While I understood the recommendation, I wasn’t entirely sure how to correctly implement pre-connect confidently.  
2. Largest Contentful Paint (LCP)
    - The LCP element was the #contact-page-background section, which contains a background image that slightly delayed loading.
    - I altered my CCS to include two photos for my background image, one for desktop and one for mobile however this was still flagged.
3. Eliminate Render-Blocking Resources
    - Bootstrap CSS (from JSDelivr CDN) and Google Fonts were flagged as render-blocking, delaying the first paint of the page.
    - These resources were necessary for the page’s styling and typography, and I didn’t know how to defer them effectively without breaking the layout.
4. Reduce Unused CSS
    - Unused styles from Bootstrap and FontAwesome were detected, increasing overall stylesheet size.
    - Bootstrap is an essential part of the design system, and I wasn’t confident in removing unused styles without affecting layout integrity.
5. Preload Largest Contentful Paint Image
    - The audit recommended preloading the background image (contact-page-background-image-medium.webp) to improve LCP.
    - Since it’s a background image, I wasn’t sure how to implement preload correctly without affecting page styling.
6. Minify CSS
    - The style.css file was flagged for minification, which could reduce its size and improve page speed.
    - While I knew how to minify CSS manually, I wasn’t sure how to automate it properly in my workflow.
7. Serve Static Assets with an Efficient Cache Policy
    - Some static assets, including the contact page background image, lacked long-term caching, meaning they were reloaded more often than necessary.
    - The site is hosted on GitHub Pages, where I have limited control over cache expiration settings.

#### Success Page

The Thank You Page achieved a 96% performance rating on desktop and an 82% performance rating on mobile. 

Despite these high score, several diagnostics were flagged:

1. Eliminate Render-Blocking Resources
    - The Bootstrap CSS from JSDelivr (1,110ms delay) and Google Fonts (780ms delay) were flagged as render-blocking, meaning they slowed down the page load time.  
    - Both Bootstrap and Google Fonts were essential for the website’s design, and I wasn’t sure how to defer them without breaking the layout.  
2. Largest Contentful Paint (LCP) 
    - The LCP element was #success-image, meaning this image was the largest visible element and took the most time to load.  
    - I did specify a height for this image, but LCP timing can still be affected by network latency and render-blocking resources.  
3. Reduce Unused CSS
    - The Bootstrap styles and FontAwesome styles were flagged for containing unused CSS rules, contributing to unnecessary page weight.  
    - Since Bootstrap is a core part of my styling, I didn’t know how to remove unused styles without breaking the layout.  
4. Minify CSS
    - The style.css file could be minified to reduce its size and improve page load speeds.  
    - I wasn’t sure how to automate CSS minification properly without affecting my development workflow.  
5. Serve Static Assets with an Efficient Cache Policy  
    - The Thank You page’s static assets (including the success image) lacked a long-term cache policy, meaning they may be reloaded unnecessarily for returning visitors.  
    - My site is hosted on GitHub Pages, where I have limited control over cache expiration policies.  

#### 404 Page

The 404 Page achieved a 99% performance rating on desktop and an 88% performance rating on mobile. 

Despite these high score, several diagnostics were flagged:

1. Eliminate Render-Blocking Resources 
    - The Bootstrap CSS from JSDelivr (940ms delay) and Google Fonts (790ms delay) were flagged as render-blocking, meaning they slowed down the page load time.
    - Both Bootstrap and Google Fonts were essential for the website’s design, and I wasn’t sure how to defer them without breaking the layout.
2. Largest Contentful Paint (LCP)
    - The LCP element was #error-image, meaning this image was the largest visible element and took the most time to load.
    - I did specify a height for this image, but LCP timing can still be affected by network latency and render-blocking resources.  
3. Reduce Unused CSS
    - The Bootstrap styles and FontAwesome styles were flagged for containing unused CSS rules, contributing to unnecessary page weight.
    - Since Bootstrap is a core part of my styling, I didn’t know how to remove unused styles without breaking the layout.
4. Minify CSS
    - The style.css file could be minified to reduce its size and improve page load speeds.
    - I wasn’t sure how to automate CSS minification properly without affecting my development workflow.
5. Serve Static Assets with an Efficient Cache Policy
    - The 404-image.webp and other static assets lacked a long-term cache policy, meaning they may be reloaded unnecessarily for returning visitors.
    - My site is hosted on GitHub Pages, where I have limited control over cache expiration policies.
6. Page Prevented Back/Forward Cache Restoration
    - The browser flagged an issue where the 404 page couldn’t be stored in the back/forward cache, making navigation slower.
    - The issue was flagged because only pages with a 2XX status code can be cached, which isn’t applicable to a 404 page.

#### **Usability and Optimization**