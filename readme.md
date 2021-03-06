# Community Choir Website —[The Singing People](https://mcglasp.github.io/the-singing-people)


**The Singing People.** A community singing group in need of a simple website that gets straight to the point.

![Initial view of homepage - showing 100vh](/readme-assets/screenshots/responsive-example.png)

## Jump to:
- [Final wireframes](#updated-wireframes)
- [Build report, testing, existing issues](#build)
- [Implementation of features resulting from user stories](#design-responses-to-user-stories)

# UX Considerations

## **Strategy**

### **Purpose**

This is the website for a laid-back community choir. They hold events every week for anyone who wants to come along and join in. The website’s approach is designed to attract a more diverse demographic than would usually be associated with community singing. As the older demographic are typically active members of community choirs whether or not the choir has an online presence, this website will be designed to appeal to a ‘mobile-first’ generation.

### **Who is it for?**

Anyone interested in joining the group. Joining a choir can feel like a big commitment, so The Singing People's focus is on being fun, casual and low-commitment. The website emphasises this both through its content, design and UX.

### **User stories**

- "As a young and enthusiastic singer I want to know how to join in, and I want that information immediately!"
- "As someone new to singing I'm nervous about joining this group, so I need to be able to sign up quickly and easily when I'm feeling confident."
- “As an active community singer I'd like to see lots of pictures that give me an idea of what this group is like — I don't want to trawl through pages of text to find out."
- “As an experienced choir member I want to hear the choir so I know that this is the kind of thing I want to do."
- "As someone with lots of other interests I can't commit right now — I'd like to check the group out on social media before I decide."
- "As a singer with previous experience I just want to turn up to the next event — when is it and where?"
- "As a busy person I want you to give me the basic info I need, and show it to me on one page on my phone — and quickly!"

### **What is the site’s value to the user?**

The site gives users the information they want in a simple and clear format. It is a single-scroll page to reduce the need to wait for further information to load. The user can jump to relevant sections and find what they need in seconds. This gives them the ability to get involved when they feel compelled to do so.

### **What is its value to me/the owner?**

Running a choir of any kind can be an admin-heavy operation. The value of this site to the owner is in reducing this admin overhead by answering the questions potential new members typically have, automating the new-member process and, potentially in a future update, creating a platform for the distribution of materials to the existing choir.

On completing the simple Join form, users would be automatically emailed out a welcome PDF, which would include the answers to a number of FAQs, saving the organisers from answering the inevitable emails which would follow! As the scope of this project extends only to front-end functionality, it has not yet been possible to implement this feature on the live site.

### **Competitors**

This website does not have ‘competitors’ in the strict sense of the word, as it is not a commercial project, but there will be other similar groups also open to new members, and most people do not have time to become involved in more than one community choir, so there is competition in that sense. Examples we can look to for inspiration (or otherwise!) include:

#### Singing Saturdays - Clear and engaging layout and presentation of information.

www.singingsaturdays.co.uk

![Singing Saturdays website screenshot](/readme-assets/screenshots/singsat-small.png)

The initial homepage view offers almost everything you’d want to know on first visiting the site. The callout tells us what this is, what the focus is, and when it is. The adjacent “Book online” indicates that it is open to anyone, and if we’re unsure we can easily navigate to the ‘About’ page in the navbar above. For anyone not certain but wanting to learn more, they can sign up to the newsletter or follow the event on Facebook. Just within view on loading is more information to scroll down to, which explains more about how these events work and why you might want to come to them.

Navigation around the site is obvious and intuitive. The links, however, when I visited the site, did not work quite as expected. Mostly they jumped to different parts of the homepage. This in itself was not a problem, but given that the information took up little space on the page, the user is forced to search for the information they are interested in. Though it may seem overcomplicated for such a simple site, this suggests it may be beneficial to separate this information to a separate page entirely with a clear and easy-to-read title.

Overall, the Singing Saturdays site brings the user value in that it answers questions easily and clearly, making the information easy to find in an intuitive and expected way, while incorporating culturally appropriate design (fun fonts, colour, and bright, engaging photos).

#### Norwich Community Choir - poorly designed and difficult to navigate.

www.norwichcommunitychoir.co.uk

![Norwich Community Choir website screenshot](/readme-assets/screenshots/norcom.png)

Though this website offers many of the basic information links that we see on the Singing Saturdays website shown above, this site fails the user in a number of ways:

The navigation section takes us quickly to different key information elements, but does so in an unnecessarily clunky way. The text is too small, and too wordy. The icons are unnecessary. Arguably, there are too many.

Overall, the site fails its target audience in its presentation. I had to work quite hard to confirm that this was a group for **both men and women**. However, the majority of the images feature only women and the colour scheme is quite traditionally ‘female’ in a way that is now quite outdated.

## **Scope**

### **Key Features**

| Feature                                      | Label | Feasibility (1-5) | Importance (1-5) |
| -------------------------------------------- | ----- | ----------------- | ---------------- |
| Basics - how we work, what we do, who we are | a     | 5                 | 5                |
| Contact /sign-up form                        | b     | 5                 | 5                |
| Future events/rehearsals                     | c     | 5                 | 5                |
| Meeting times                                | d     | 5                 | 5                |
| Music download                               | e     | 4                 | 3                |
| Links to songs to learn                      | f     | 5                 | 3                |
| Shop - group t-shirts etc.                   | g     | 1                 | 1                |
| Personnel page - key stakeholders etc        | h     | 4                 | 2                |
| Gallery                                      | i     | 5                 | 5                |
| Blog - event write-ups, announcements        | j     | 2                 | 1                |
| Members’ area                                | k     | 1                 | 2                |


![Feasibility v Importance Feature Graph](/readme-assets/screenshots/feasibility-importance-graph.png)


Plotting the feasibility scores of potential features against their importance demonstrates that my focus should be on the following:

**High priority**

- Basics (who, what, where, etc.)
- Contact form
- Future Performances
- Meeting times
- Gallery

**Medium Priority (nice to have)**

- Sheet music download
- Links to recordings/videos
- Key personnel

We can clearly see that the following should not be attempted in the initial development of the site:

**Low priority (future development)**

- Online store
- Blog
- Members’ area

## **Structure**

This community choir wishes to broaden its member base out from the stereotypical over-50s female, while still being accessible to that demographic. The site will therefore be designed with the mobile-first methodology, to cater for a demographic with less time and poorer access to desktop or laptop devices. It will remain clear and accessible when viewed on a larger screen so that the site remains accessible and welcoming to all.

### **Navigation**

Fundamental user questions to answer on loading the site:

- Who and what we are
- Where and when we do it
- How you join us

Potential layouts to facilitate the above structure

- navbar (Inline. Reduce to toggler on mobile)
   - Who/what/how
   - Where/when
   - Gallery
   - Join

- hero image
— ‘Join us’ button overlaid? 
- Stack sections with basic info as per navbar. 
Clickable to further info.
- Social media links
- Footer


## **Skeleton**

### **Initial Wireframes**

Mobile First mockup, created with Balsamiq.
[Mobile First mockup](/readme-assets/wireframes/mobile-first.png)

Desktop mockup, created with Balsamiq.
[Desktop mockup](/readme-assets/wireframes/desktop.png)

### **Updated Wireframes**

On beginning to create the live site, it became clear that certain elements of my wireframes would not work in reality. These were updated, as linked to below, to more accurately guide development.

The updated Desktop design is brought more in line with the design of the mobile version, whereby a user scrolls sequentially through the information sections, rather than stacking them side-by-side. This allows for bigger, clearer and easier-to-read text, and for the links to jump directly to the correct section, allowing users to get to the information they want more quickly. I also decided to present the images in a carousel so that they can be skipped past quickly if this is not what the user is interested in; the entire gallery is accessible but only takes up one image's-worth of space.

Mobile First mockup, created with Balsamiq.
[Mobile First mockup](/readme-assets/wireframes/updated-mobile.png)

![Mobile First mockup](/readme-assets/wireframes/mobile-first-inline.png)

Desktop mockup, created with Balsamiq.
[Desktop mockup](/readme-assets/wireframes/updated-desktop.png)

![Desktop mockup](/readme-assets/wireframes/desktop-inline.png)

## **Surface**

### **Colours & Fonts**

By exploring other community and singing websites, I found that colour-schemes were friendly, unchallenging and, largely, fairly unsubtle. Soft blues and reds were being used on sites that had clearly been professionally designed. I found that by using these sorts of colours I could more easily keep the site gender and age neutral, which is extremely important for this group. The blue also served the design by being easy to work into a background, without compromising contrast ratios, while the red could be used for buttons and other 'call-to-action' elements.

The heading font I used felt casual and fun, which seemed right in the contexts I've described above. The ‘sketched’ quality emphasises the casual nature that is core to this group's approach.

The body font was initially a serif font, which contrasted nicely with the heading font, but was slightly too difficult to read. I decided to change this to a sans-serif font, which still contrasts well but is far more legible.

### **Design responses to user stories**

"As a young and enthusiastic singer I want to know how to join in, and I want that information immediately!"

![How to join in](/readme-assets/screenshots/how.png)

*Almost immediately accessible via minimal scrolling is this section, clearly stating its purpose and encouraging interaction from the user.*

"As someone new to singing I'm nervous about joining this group, so I need to be able to sign up quickly and easily when I'm feeling confident."

![Joining form](/readme-assets/screenshots/join.png)

*Several links, including one in the navbar and a large 'Join' button both visible on page load jump to this form. The buttons are clear in their purpose — 'Join in!' or 'Join us'. The form only requires three inputs from the user.*

“As an active community singer I'd like to see lots of pictures that give me an idea of what this group is like — I don't want to trawl through pages of text to find out."

![Image carousel](/readme-assets/screenshots/carousel.png)

*The site has a dedicated gallery, of course, but I have also been sure to illustrate every section with a striking image, where at all practical from a design perspective. The inclusion of these images alongside frequent invitations to get involved should give the user a positive reaction to exploring the site.*

“As an experienced choir member I want to hear the choir so I know that this is the kind of thing I want to do."

![Embedded video](/readme-assets/screenshots/watch.png)

*Users do not have to search for long to see what they might be joining, but they can easily skip past this content if they don't want to watch the video; it is not automatically played.*

"As someone with lots of other interests I can't commit right now — I'd like to check the group out on social media before I decide."

![Fixed social media element](/readme-assets/screenshots/follow-fixed.png)

*I initially left the social media links at the very bottom of the scrolling page, as I felt they were not a top priority. I later made the decision to add a small 'fixed' set of icons to the left bottom corner of the site, which scrolls with the user. This gives immediate access to follow the group for anyone on the fence about joining up.*

"As a singer with previous experience I just want to turn up to the next event — when is it and where?"

![When and where?](/readme-assets/screenshots/when-where.jpg)

*Event information is clearly laid out, illustrated and easy to find.*

"As a busy person I want you to give me the basic info I need, and show it to me on one page on my phone — and quickly!"

![Navbar dropdown menu](/readme-assets/screenshots/dropdown-nav.png)

*At the top of the mobile view is a toggler (hamburger icon) which displays links to all the group's essential information.*
# Build

## Technologies used

Languages:
- HTML5
- CSS3
- Javascript

Integrations & Libraries
- JQuery
- Bootstrap
- Google fonts
- Fontawesome

Build, Version control & Deployment:
- Gitpod - for building. Incorporated several IDE extensions, including Auto Close Tag, Bootstrap 4CDN Snippet, HTMLHint, Prettier and Live Server.
- Github - Version control
- Gitpages - Cloud hosting
- Browsers used for build and testing: Chrome (including mobile), Firefox, Safari (including mobile)

## Testing

There are several elements to focus on in testing the site:

- Responsiveness
- Accessibility
- Validation
- Images
- Internal links
- External links
- CSS transitions
- Scripts

### Testing Plan & Results

- **Checked responsiveness** while building both mobile and desktop sites using three tools: Chrome developer tools, responsinator.com and amiresponsive.is. Checked for responsiveness errors across all given devices, including the Responsive tool available on Chrome; landscape views were included. All page elements display as expected with regard to CSS media queries and Bootstrap classes. I found and fixed a lack of padding around a recently added carousel container. I added a media query to change the nature of elements on devices below 400px wide, eg. the Galaxy Fold. By reducing padding on the .border class I found that more content was available to the user and the layout generally improved. On these screen sizes I also changed some attributes of the .circle class, as these elements were escaping their containers at this size.
- **Ensured accessibility standards are met.** I manually checked code for 'alt' attributes on images, or sr-only classes, where necessary. Google’s Lighthouse tool on Chrome was used to evaluate accessibility. The result was 97%, revealing the navigation links to have insufficient contrast ratio. This was corrected to bring it into line with minimum standards.
- **Copied all CSS and HTML code to Jigsaw/W3 Schools CSS and HTML validators.** This returned warnings relating to the comments used in my HTML code ('The document is not mappable to XML 1.0 due to two consecutive hyphens in a comment.'), so these were altered. I should note that I had used this tool throughout development to correct errors and warnings to avoid replicating them throughout the site.
- On the mobile version a hamburger icon is used to toggle the navigation links. I added some code to automatically collapse this once the user has clicked, otherwise it obscured the content.
- Manually **checked all images to ensure they are displaying at an appropriate resolution** and maintaining the correct aspect ratio, which they were.
- Checked that all **internal links** jumped to appropriate positions, and that they worked. The section headings were obscured by the collapsed, fixed navbar. I added some ‘hidden’ divs to anchor the links to more appropriate places. When testing on an actual iOS device, unusual behaviour was found with the anchor tags. See 'Existing Bugs' below for more information. 
- Ensured that **external links open to a new tab** and land on the correct URL. I found that my Instagram Fontawesome icon was actually directing to Twitter. This has been corrected.
- Tested CSS/Javascript navbar transition across several browsers. I found that, regardless of the browser used, if I stopped scrolling at a very specific point, the navbar jumped continuously between two states. As this is a very minor design issue, and does not affect functionality, I will investigate this further during future development and when my Javascript skills are improved.

The above steps were completed in Chrome, Safari and Firefox browsers, and using real devices where possible. Most elements appeared and functioned identically across all three browsers, though there were CSS elements being overridden in Safari. I updated the browser version, which fixed a number of problems, though running the CSS code through an Autoprefixer (as listed below) solved other minor issues.

### Existing compromises & areas for future development

My first priority for future development, and when my Javascript skills allow, will be to add a modal popup confirming the user has correctly completed the sign-up form. This was originally included in the build, but I found that I was unable to have the form complete validation of required fields and have the appearance of the modal be dependent on the results of these tests — instead, the modal appeared whether the form had been correctly completed or not. More detailed Javascript will be required for this functionality, but it is crucial to the user's positive interaction with the site to receive this kind of feedback, and it is therefore my intention to add this feature.

### Existing bugs

 - Navbar behaviour on iPhone/iPad: actual devices

The problem of the fixed navbar obscuring headings was addressed by offsetting the anchor tags by a number of pixels to correct for the height of the navbar. This worked perfectly on all screen sizes in Chrome developer tools. However, when viewed on an actual device, I found that the navbar's behaviour was different. Specifically, it pushed the content down, rather than overlapping it. When a link was selected, it then pulled the content back up with it, thereby taking the user to content far below the anchor tag. The solutions I tried for this were extensive and included:
- CSS media queries specifically designed to target iOS devices.
- Experimenting with different implementations of the same approach within CSS.
- Moving the anchor tags to different places within the HTML.
- Using JavaScript and JQuery to implement the offset.

The problem was discussed at length with two Code Institute tutors who were unable to identify the cause of the problem. I was advised by both tutors to outline the issue here and submit the project with the existing functionality, marking the problem as an area for future investigation.

 - 'Join us!' buttons maintain :hover state on mobile view

 This problem appeared suddenly - literally over night - when there had been no changes made to these or related classes. The bug is this: the red button turns blue when hovered over, which is correct. However, once clicked, it maintains that colour until something else on the page is clicked. To rectify this I looked closely at all colour-related CSS styles, checked for rogue Javascript code, Googled the issue and eventually discussed it with a Code Institute tutor. He was also unable to account for it and we concluded that the bug was likely to be coming from a change to the core Bootstrap styling. As the issue is purely cosmetic, does not compromise the design, and appeared apparently randomly, I have marked it down as an area to review in future development.

## Deployment

The site was deployed directly from the Github repository, using Github Pages. When initially made live, I found that the site was not displaying all elements in the expected way. Some research into this revealed that a line of code was needed in the head section for Github Pages to render the site correctly. This snippet of code is credited in the index.html file.

To deploy the site, it was necessary to undertake the following steps:

- Access the repository at https://github.com/mcglasp/the-singing-people
- Click on the repository settings
- First ensure that the name of the repository is satisfactory and appropriate to be used as the URL for the live site
- Scroll to the Github Pages section
- Select the master branch as the source and the /root folder
- Save
- Navigate to the newly created URL (as per the name of the repository or custom domain) and ensure that the live site displays as expected and identically to the preview version


# Online Resources

I used the online resources below for general guidance and solutions to specific problems. Specific coding solutions are also signposted in HTML and CSS comments.

- Code Institute Full Stack Development course material, mentor and tutors.
- Slack community (specific solutions to coding problems and general guidance)
- Stack Overflow website (specific solutions to coding problems)
- CSS-tricks (specific solutions to coding problems)
- Codepen (specific solutions to coding problems)
- Freecodecamp (specific solutions to coding problems)
- W3 Schools (specific code examples and tutorials)
- The Responsinator (check responsiveness)
- AmIResponsive (check responsiveness)
- Autoprefixer CSS online (increase compatibility across browsers)
- Jigsaw and W3 Schools (code validators)
- Google Chrome (development tools)
- Webaim.org (accessibility guidance)
- favicon.io (favicon generator)


# Credits & Acknowledgements

All photographic and video content was created either by myself or attendees of the annual Stephen Taberner Singing Weekends.

A small amount of code was provided by forum users from several websites (see below).

Thanks to the following Stack Overflow users for their guidance in solving various issues as credited in the HTML, CSS and Javascript code:

- Julian S, Sean, Vadim Ovchinnikov, George Kagan, Eric Olsen

Thanks also to:
- Freecodecamp user ellereeeeee
- Sitepoint user Paul OB
- Bootstrap Studio user buntonn

Thanks also to my mentor Antonio Rodriguez, the Code Institute Tutors, Jim Lynx and the Slack community.

