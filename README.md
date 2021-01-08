# Create your Personal Project Page
In this series of steps, you'll utilize an existing CSS to create a webpage to serve as your mobile resume. 

## Pick Your Style
The current color scheme is listed at the top of the `style.css` file. Take some time to decide on a color scheme you would like to use. Stick with 2 to 4 colors beyond the background color. 

- **TO DO** Search [Color Hunt](https://colorhunt.co/) or [W3Schools Pallettes](https://www.w3schools.com/colors/colors_palettes.asp). Change all the existing colors in the `style.css` page to use your selected colors. 

There are two font styles chosen so far: Lucida Sans and Courier New. As each web browser supports different font styles, you'll notice that several fonts are listed for each selection. The browser will attempt to load the first font. If it cannot be found, then it will go down the list until it finds a supported font. 

```
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
```

- **TO DO** Search [CSS fonts](https://www.w3.org/Style/Examples/007/fonts.en.html) for fonts to choose from and the accepted default if it is not supported. Replace the `font-family` with your desired font. 


## Create Your HTML Sections
The webpage will contain four sections: the top section is the `header`, the middle section will be a `row` and contains the menu and then the page contents, and finally the bottom section is the `footer`. 
- **TO DO** In the `index.html` file, locate the `body` tag and add the following: 
```
    <body>
        <div class="header">
        </div>
        
        <div class="row">
        </div>
        
        <div class="footer">
        </div>
    </body>
```

### Middle Section - Row 
In this section, you can decide to make two or three columns for information. The first column will serve as a navigation and the second column will contain information about your skills, education, and projects. If you choose, the third section can be used for social media, an image or you, or even an important quote. 

Observe the multiple column classes in `style.css`. When choosing column widths, you must make sure that all columns selected add up to 12. For two columns, consider using `col-3` and `col-9` to have one small and one large column. For three columns, use `col-3` and `col-6` and `col-3` to have one large middle column and two small columns on each side. 

The example code below is for only 2 columns. Adjusted for your preference. 
- **TO DO** Inside the `row` section, add two new `div` sections using the correct column size. The `div` section should also include the `menu` presets. 

```
  <div class="row">  /* code already exists */
    <div class="col-3 menu">
    </div>

    <div class="col-9">
    </div>
  </div>    /* code already exists */
```

## Adding Content 
In each of the following sections, you will add the text to your project. From this point on, you should press **RUN** after each TO DO step you have completed to check your work. 

### Header 
In this section, we'll add your name as the title. 
- **TO DO** Include an `h1` tag with your name inside the header `div`. 

```
    <div class="header">
      <h1> Your Name </h1> <!-- Add this line, use your name -->
    </div>
```
Press **RUN** to preview. Consider changing the font style or color in the `h1` tag in the `style.css`. 

### Menu 
In this section, we will add the buttons to navigate through the page. Find the existing right column `div` tag. Inside that tag will be an unordered list with several list items. Each list item is formatted as a button. See the `.menu ul` and `.menu li` and `.menu a` rule sets in `style.css` to see how these tags are personalized to the menu class. 

You will need to consider what categories you want to include. I will be using *About*, *Education*, *Experience*, and *Community*. You may consider changing the names of these and use anything from the table below. 

| Category | What to include | Other Titles |
| --- | --- | --- |
| About | Give a statement of your goals, what type of job you are interested in, and if you have hobbies that are relevant to your job goals | Objective, Introduction, Hello World |
| Education | Provide information about school. May also include conferences, workshops, or camps you have attended | Training, Skills |
| Experience | Include work you have done - paid or unpaid - that has built your job skills or interpersonal skills. You may also include descriptions and links (if possible) to personal projects you have completed. | Projects, Work Experience |
| Community | This section is an opportunity to tell people about groups you are involved with and how you help others. | Activities, Volunteer Experience |

- **TO DO** Include the following list inside the `div` tag for menu. It is ok to use different names. Each list element will link to a section of the page, remember the ID's you use here for the sections later. 

```
    <div class="col-3 menu">  /* code already exists */
      <ul>
        <li><a href="#about">ABOUT</a></li>
        <li><a href="#edu">EDUCATION</a></li>
        <li><a href="#exp">EXPERIENCE</a></li>
        <li><a href="#comm">COMMUNITY</a></li>
      </ul>
    </div>    /* code already exists */
```

### About Content 
Now to include your details!  This is really where you sell yourself. We will use the largest `div` section inside the `row` to add titles and content. Let's start with the *About* section. 

Each section will be linked to the Menu. For that, it is necessary to use the `a` tag for the heading so it is linked to the appropriate button in the menu. **NOTE** Make sure the `id` you use here matches the `href` in the corresponding menu button. 

- **TO DO** Find the largest column section inside the `div` tag for the `row`. Add a title using the `a` tag followed by the `h1` tag. Next, include a `p` tag with information about yourself. Finally, include a link that will navigate the user back to the top of the page. This is helpful for when your page includes lots of content. 

```
    <div class="col-9">   /* code already exists */
      <a id="about"><h1>HELLO WORLD</h1></a>
      <p>I like creating.</p>
      <a href="index.html" class="home">Back to top</a>

    </div>   /* code already exists */
```

Preview your page. You can go to `style.css` to change any fonts or colors for this section. 

### More Sections 

Time to include more sections! Next up is the *Education* section. Here, you should include the name of the school, the dates, and a small description of what classes you participated in. You may also decide to include GPA, clubs, and any honors you received. 

- **TO DO** Right below the *About* section, add another `a` and `h1` title for *Education*. Next use one of the smaller heading tags, like `h3` to display the school name. After this, use an unordered list or paragraph to add details. Below are a few suggestions for your education section. 

**OPTION 1**
```
      <a id="edu"><h1>EDUCATION</h1></a>
      <h3> SchoolName High School </h3>
      <h4> August 2000 to Present </h4>
      <p>Courses include German, Peer Tutoring, and Forensics. Member of the  </p>
      <a href="index.html" class="home">Back to top</a>
```

**OPTION 2**
```
      <a id="edu"><h1>EDUCATION</h1></a>
      <h3> SchoolName High School </h3>
      <h4> August 2000 to Present </h4>
      <p> Activities include: </p>
      <ul>  
        <li>Completed 3 AP courses and 6 Honors courses</li>
        <li>Member of the INTERalliance</li>
        <li>Member of Marching Band and Pep Band</li>
      </ul>
      <a href="index.html" class="home">Back to top</a>
```

- **TO DO** From here, use a similar format to add *Experience* and *Community* sections. 

## Wrapping Up

Continue adding content to the page. You may consider adding more categories to your middle content, adding a favorite quote, or adding images. 
