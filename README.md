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
### Header 
In this section, we'll add your name as the title. 
- **TO DO** Include an `h1` tag with your name inside the header `div`. 

```
    <div class="header">
      <h1> Your Name </h1> <!-- Replace this line -->
    </div>
```
From this point on, you should press **RUN** after each TO DO step you have completed to check your work. For this section, consider changing the font style or color in the `h1` tag in the `style.css`. 

### Middle Section - Row 
In this section, you can decide to make two or three columns for information. The first column will serve as a navigation and the second column will contain information about your skills, education, and projects. If you choose, the third section can be used for social media, an image or you, or even an important quote. 

Observe the multiple column classes in `style.css`. When choosing column widths, you must make sure that all columns selected add up to 12. 

## Wrapping Up

From this project, you can branch off to add extra pages. At least one page should be devoted to your own projects you have made. 
