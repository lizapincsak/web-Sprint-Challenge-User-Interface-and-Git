
# Sprint Challenge: User Interface and Git - Multi-Page Website

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a concrete project. This Sprint explored User Interface and Git. During this Sprint, you studied Semantic HTML, CSS Fundamentals, CSS Flexbox Module, and Git. In your challenge this week, you will demonstrate proficiency by creating a multi page website that has some missing HTML elements as well as CSS specificity problems that need to be solved.  You will also create an additional web page that will be linked to from a navigation you will build.

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your TL if you need direction. Your work reflects your proficiency in user interface and your command of the concepts and techniques in semantic HTML, CSS fundamentals, CSS flexbox module, and git.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons and your project manager.

## Description

In this challenge, you build a missing header (navigation and image) on the home page, update some CSS styling on the home page, and create an additional page (About) which will link from the navigation you created.

In meeting the minimum viable product (MVP) specifications listed below, your web page should look like the solution screen shots of the home and about pages (found in the design-files folder):

[Click here for the home page example](https://tk-assets.lambdaschool.com/39a49225-8ac9-43da-aa90-514fd60ae99a_sprint-challenge-ui-home-example.png)

[Click here for the about page example](https://tk-assets.lambdaschool.com/ede1bb1a-63ff-4801-8c02-3efa2f603190_sprint-challenge-ui-about-example.png)

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your Team Lead

1. If you were to describe semantic HTML to the next cohort of students, what would you say?

Semantic HTML is a way to give meaning to the content that you want to display on the page. You use HTML to communicate with CSS, which is the design portion of the webpage. HTML is the structure/backbone of the hosue, and CSS is the interior and exterior design of the house. 

2. Name two big differences between ```display: block;``` and ```display: inline;```.

Two big difference between display: block and display: inline is:
    1. With display: inline, the width and height are not respected. The element will end up on top of another element. The padding will still be present but may over lap. But, they will sit side-by-side. 
    2. With display:block, width, height and padding are respected. However, the elements will not align next to each other. 

    The main difference is that display:block will have width, height and padding respect, but the elements will not be next to each other. While, display:inline will not have width and height respected, but the elements will be next to each other. 

3. What are the 4 areas of the box model?

The four areas of the box model are: 
    1. Content edges
    2. Padding edges
    3. Border edges
    4. Margin edges

4. While using flexbox, what axis does the following property work on: ```align-items: center```?

Aligh-items: center uses the cross axis. 

5. Explain why git is valuable to a team of developers.

Git is valuable to a team of developers because multiple people can work on the same project at the same time. When you branch the project, you can work on your own portion of the project, and when you add what you've created the branches will merge back together. Additionally, someone can work on an aspect of a branch that you're working on by creating another branch. This entire process of brancching and growing back together can continuously happen until the project is complete. 

You are expected to be able to answer all these questions. Your responses contribute to your Sprint Challenge grade. Skipping this section *will* prevent you from passing this challenge.

## Project Set Up

- [ ] Create a forked copy of this project.
- [ ] Add your Team Lead as collaborator on Github.
- [ ] Clone your OWN version of the repository (Not Lambda's by mistake!).
- [ ] Create a new branch: git checkout -b `<firstName-lastName>`.
- [ ] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
- [ ] Push commits: git push -u origin `<firstName-lastName>`.
 
Follow these steps for completing your project.

- [ ] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo). **Please don't merge your own pull request**
- [ ] Add your Team Lead as a reviewer on the pull-request
- [ ] Your Team Lead will count the project as complete by merging the branch back into master.
 


## Minimum Viable Product

Your finished project must include all of the following requirements:

### Home Page

[Review the provided design file for the home page](design-files/home.png).  Notice the navigation and header images are missing.

* [ ] Build the HTML and CSS to create the missing navigation and header.
* [ ] Link the `About` navigation item to the [about.html](about.html) page

You will also notice there are 10 boxes on the home page that need background colors.  Use this list below to correctly style each box:


### About Page

[Review the provided design file for the about page](design-files/about.png). You have been provided the HTML wrapper, footer, and page content for the about page. Create the rest of the missing HTML and CSS to match the design file.



* [ ] Build the rest of the about page layout to match the design

In your solution, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

Note: Please make sure you are using flexbox to layout your website. Floats, inline-block, tables, etc, should not be used for layout. 

## Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on the following optional goals:

* [ ] refactor your HTML, make sure it's indented properly, clean, readable, you have written appropriate comments where necessary and that all attributes (required and encouraged) are filled out correctly.  
* [ ] Ensure your CSS is organized and readable, you've seperated your code by section and that you are using descriptive class names and adding classes in your HTML where styles repeat rather than rewrting the same styles over again
* [ ] Use a flex item property of your choice when laying out a section of your website, ensure you can explain how and why you've used this property 


.about{
    padding: 2%;
    border-bottom: 1px dotted black;
    margin: 4%;
    
}
.bottom-content {
    display: flex;
    margin: 0 2% 20px;
    word-wrap: break-word;
    justify-content: space-around;
    flex-wrap: wrap;

}

.bottom-content .text-container {
    height: 30vh;
    padding-right: 4%;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;

}

.bottom-content .text-container:last-child {
    padding-right: 0;
    display: flex;
    width: 32%;
    margin: 2%;
    flex-wrap: wrap;
    justify-content: center;
    text-align: justify;

}

footer {
    width: 100%;
    background: black;
}

footer nav {
    width: 60%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 2%;
    font-size: 14px;
}

footer nav a {
    color: white;
    text-decoration: none;
}.img{
    height: 20%;
    margin: 10px;
    padding: 4% 0;
}