Understanding HTML and CSS Structures for Effective Web Scraping

* * * * *

### Objective:

The goal of this assignment is to:

1.  Understand how HTML and CSS are used to structure and style web pages.

2.  Learn to analyze and navigate the Document Object Model (DOM) to identify the data to be scraped.

3.  Gain hands-on experience in simulating data extraction from a webpage using web scraping tools.

* * * * *

### Part 1: HTML Basics

1.  Create a Static Webpage

     Design a simple HTML webpage for a movie review platform. Include the following elements:

     - A header with the platform's name.


     - A table displaying the following information about 5 movies:

        - Movie name

        -   Genre

        -   Duration

        -   Release year

        -   Rating

        -   Trailer

-   Required data is available in  [movies.json](./movies.json)

Example structure
```
<table border="1" cellspacing="0" cellpadding="5">

    <tr>

        <th>Movie Name</th>

        <th>Genre(s)</th>

        <th>Duration</th>

        <th>Release Year</th>

        <th>IMDB Rating</th>

        <th>Trailer</th>

    </tr>

    <tr>

        <td>The Dark Knight</td>

        <td>Action, Romance, Comedy</td>

        <td>3 hrs</td>

        <td>2008</td>

        <td>9.0</td>

        <td>

            <iframe 

                src="https://www.youtube.com/embed/dQw4w9WgXcQ" 

                allowfullscreen 

                title="The Dark Knight Trailer" 

                width="200" 

                height="113" 

                frameborder="0">

            </iframe>

        </td>

    </tr>

</table>
```

2.  Add unique classes and IDs to key elements for styling and identification during scraping.

* * * * *

### Part 2: CSS Integration

1.  Style the Webpage

    -   Use CSS to enhance the appearance of the webpage.

    -   Add the following styles:

            -   A consistent font across the webpage.

            -   Borders and alternating row colors in the movie table

    -   Any other styling you like

* * * * *

### Part 3: Analyze for Scraping

1.  Identify Data Points

    -   Analyze the DOM structure of the webpage you created.

    -   List the CSS selectors (e.g., #movie-table, .movie-name) to access each of the data points (e.g., movie name, genre).

    Example:

    Selector for movie name: `.movie-name`

2.  Explain the Role of Attributes

    -   Highlight how unique attributes like id and class help scraping tools locate elements on a webpage.

### Deliverables:

-   The HTML and CSS files for the static webpage.

-   A document having the following things

    1.  Screenshot of the web-page you created
    
    2.  Analysis of the DOM structure
    
    3.  List of CSS Selectors
    
    4.  Briefly explain the role of atrributes