#  CSS-enhanced Personal Portfolio project

In this CSS-enhanced Personal Portfolio project, you'll elevate your online presence by crafting a visually stunning and engaging personal portfolio website. This project builds upon the foundation of your existing HTML portfolio, transforming it into an eye-catching and interactive showcase of your talents and accomplishments.


##### Project Requirements (this is building upon your portfolio from last week, only new content should be your CSS):

1. Home Page:
    - The main landing page provides an introduction to you and your portfolio.
    - Include a brief bio, your name, a profile picture, and a welcome message.
    - Apply a visually appealing color scheme and typography to create an      inviting and professional welcome message.
    - Style your profile picture for an aesthetically pleasing presentation utilizing rounded corners, and shadows. 


``` html
    <link rel="stylesheet" href="style.css">
 
</head>
<body class="main">
    <header align="center">
        <h1>Welcome to The Dr. Strange Portfolio</h1>
        <p> Sorcerer Supreme - Earth's foremost protector against magical and mystical threats</p>

        <hr>
        <nav>
            <a href="aboutme_pg.html">About Me</a>
            <a href="resume_pg.html">My Resume</a>
            <a href="contact_pg.html">Contact me</a>
            <a href="recomend_pg.html">Testimonials/Recommendation</a>
        </nav>
            
    </header>
    <br>

    <img
    src="images/dr_strange_main photo.jpeg"
    alt="image of Dr.Stange using the time stone"
    class="center"
    >
    <hr>

    <footer>
    <h4 class="mini_bio" align="center" >
        Embark with us on a mystical journey to explore the Sorcerer Supreme himself.....
    </h4>
    </footer>
</body>

```
#### CSS code:

``` css
body{
    background: black;
    color: white;
}

.main{
    display: grid;
 
}

.center{
    border-radius: 50%;
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

  .mini_bio{
    color: white;
  }

  header nav a{
    color: green;
    font-size: 1.3em;
    margin: 1em;
  }
  ```

2. About Page.
    - A page that offers more detailed information about yourself.
    - Enhance text content with advanced typography techniques for improved readability and visual appeal.
    - Use CSS to format and structure the page to present your background, education, career goals, and personal interests in an organized manner.

``` css
    .aboutme{
    color: green
  }

.aboutme_banner{
    width: 1000px;
    height: 350px;
    display: block;
    margin-left: auto;
    margin-right: auto;
}

 .b1{
    color: firebrick;
}

.b2{
    color: firebrick;
}

.b3{
    color: firebrick;
}

.b4{
    color:firebrick
}

```
3. Resume/CV Page:


- Display your professional resume or curriculum vitae (bonus).
- List your education, work experience, skills, certifications, and achievements (at least 3).
- Highlight your technical skills, languages, frameworks, and software proficiency (at least 3) 
- You can use a visual representation like a skill bar or chart (bonus) 
- Create a well-structured layout for your resume or curriculum using CSS.
- Apply styling to highlight key information such as education, work experience, skills, certifications, and achievements (at least 3).
- Implement media queries to ensure responsiveness for both desktop and mobile devices (at least 1 per page) 

``` css
.resume{
    color: green
  }

  #resume_block{
    box-sizing: border-box;
    width: 900px;
    padding: 30px;
    border: 10px solid #eb7804;
    margin: auto;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;

}

@media screen and (max-width: 600px) {
    #resume_block{
        display: grid;
        grid-template-columns: 100%;
        grid-template-rows: 100px 100px;
        gap: 5px;
        width: 95%;
        text-wrap: wrap;
    }
}
```

4. Contact Page: 
- Provide a way for visitors to get in touch with you.
- Include a contact form, your email address, and links to your social media profiles.
- Apply CSS to create an attractive and user-friendly contact form.
- Style links to social media profiles and ensure they are visually distinguishable.

``` css
#contact_box{
    box-sizing: border-box;
    width: 900px;
    padding: 30px;
    border: 10px solid #b88307;
    margin: auto;
    box-shadow: 5px 10px #edb8b8;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color:rgb(31, 32, 31);
    color: aquamarine;
}

@media screen and (max-width: 600px) {
    #contact_box{
        display: grid;
        grid-template-columns: 100%;
        grid-template-rows: 100px 100px;
        gap: 5px;
        width: 9%;
    }
}
```

### Additional Requirements:

- All nav links must work correctly and navigate to their respective pages.
``` html
<nav>
    <a href="aboutme_pg.html">About Me</a>
    <a href="resume_pg.html">My Resume</a>
    <a href="contact_pg.html">Contact me</a>
    <a href="recomend_pg.html">Testimonials/Recommendation</a>
</nav>
```

- Use semantic elements like header, nav, main, section, article, footer for proper content structure.

``` html
<br><br>
    <section>
        <h3 class="b1" > Early years</h3>
        <article>
            Stephen Vincent Strange, M.D., Ph.D., is a brilliant but highly.....
            <br><br>
         </article>
```
- Utilize unordered lists ul and/or ordered lists ol as needed for organizing content within recommend_pg.html
``` html
<div class="review_box">

       <h1 align="center" class="reviews">Testimonials/Recommendation</h1>

        <h3 style="font-family:cursive; color: rgb(232, 139, 26); margin: auto;font-size: larger;">Reviews:</h3>
       
        <ol>
            <li>Wong:</li>
                <p>"Doctor Strange is the best of us...<p>
        <ol>
```
- Implement pseudoclasses like :hover, :active, and :focus for enhanced user interaction.
    - ultize the hover and focus pseudoclasses. 
        - hover pseudoclasses was used on my navigation selectors to shift from page to page.
        - focus pseudoclasses was used on my contact me page for the input inquriea.

``` css
nav a:hover {
background-color: aquamarine;
}

input:focus{
    background-color: rgb(248, 240, 77);
}
```

- Ensure proper spacing between and within elements using the CSS Box Model (content, padding, border, margin). used in my resume resume page.

``` css
.resume{
    color: green
  }

  #resume_block{
    box-sizing: border-box;
    width: 900px;
    padding: 30px;
    border: 10px solid #eb7804;
    margin: auto;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;

}
```

- Utilize either CSS Flexbox or CSS Grid for laying out each page, including appropriate properties and settings for each.
    - Example of a css grid being used for my Testimonials/Recommendation page.


``` css
.review_box{
    display: grid;
    width: 80%;
    border: 1px solid white;
    margin: auto;
    grid-template-columns: 1fr;

}
```

- Implement media queries to ensure responsiveness for both desktop and mobile devices (at least 1 per page) 

``` css
@media screen and (max-width: 500px) {
    .main{
        display: grid;
        grid-template-columns: 100%;
        grid-template-rows: 100px 100px 100px;
        gap: 5px;
        width: 95%;
    }
}

@media screen and (max-width: 600px) {
    #contact_box{
        display: grid;
        grid-template-columns: 100%;
        grid-template-rows: 100px 100px;
        gap: 5px;
        width: 9%;
    }
}

@media screen and (max-width: 600px) {
    #resume_block{
        display: grid;
        grid-template-columns: 100%;
        grid-template-rows: 100px 100px;
        gap: 5px;
        width: 95%;
        text-wrap: wrap;
    }
}

@media screen and (max-width: 600px) {
    .review_box{
        display: grid;
        grid-template-columns: 100%;
        grid-template-rows: 100px 100px;
        gap: 5px;
        width: 95%;
        text-wrap: wrap;
    }
}
```

