Example (showing reflection of one module):
Learning Audit for Front End only.

- Semantic HTML and Basic of CSS Layouts (RED)
- DOM selectors (RED)
- Button click and Form Submit (GREEN)
- Fetch (ORANGE)
- Async JavaScript (GREEN)
- Async/Await (ORANGE)

Learning Plan and Priorities

Semantic HTML / CSS Layouts:
Found it hard to put into practice. I wasn’t sure when to use certain tags. I need to build a few more websites with HTML to get used too quickly and correctly structuring a page.
CSS Grid was ok, I could build basic stuff. But I found Flexbox quite difficult and all I wanted to do was align some items. I want to practice making a website header with a logo, navigation list and button.
DOM
I was able to get DOM nodes but found it hard to change text values in nodes. I need write some simple JS that selects DOM nodes and reads text or html attributes.
Fetch
I could write a simple fetch request but I found error handling hard. I still don’t get how it works. I want to write a small script to get data from an API but I’ll turn off my internet to see how to handle errors (like no internet)

------------------------------------------------------------------------

Week 3 - Front End Engineering:

- Semantic HTML (GREEN)
- CSS Flexbox & Grid (AMBER)
- Selecting DOM elements (GREEN)
- Manipulating DOM elements (AMBER)
- Event listeners (AMBER)
- Asynchronous JavaScript and functions (GREEN)

------------------------------------------------------------------------

Week 4 - Back End Engineering:

- node and npm (GREEN)
- RESTful APIs (RED)
- Server to client and API relationship (GREEN)
- requests and HTTP methods (AMBER)

------------------------------------------------------------------------

Week 5 - Database Engineering:

- Intro to Databases (GREEN)
- SQL commands and functions (GREEN)
- Joins - self-joins (AMBER)
- .env files and environment variables (RED)
- pg package (node) and pool.query injections (RED)

Learning Audit for Week 5 - Database Engineering:

- Since my group in week 4 didn't get do the PUT, PATCH, or DELETE HTTP methods,
I will work on the hackathon from week 5 because this way I can practice my pool.query injections as well
as work on the HTTP methods.


![alt text](<../screenshots/Screenshot 2024-08-04 102726.png>)

Screenshot of my albums.js file in the hackathon for week 5. Since our group only did the
get and post functions for the artists, it took me a while to get the post function for 
albums to work because the albums table has 3 columns as opposed to just one.


![alt text](<../screenshots/Screenshot 2024-08-04 102944.png>)

Screenshot of ChatGPT which I used to help me understand the pool.query code a bit better:
I was wondering whether the parametrized values in the array had to match character for characer
with the names of the table columns where I was trying to insert the data into.
However, it does not matter. All that matters is the order of the elements in the array
as that is how js will associate the corresponding values.

![alt text](<../screenshots/Screenshot 2024-08-05 083035.png>)

Screenshot of my artists.js file in the hackathon for week 5. I managed to get the patch
request event handler as well as the updateArtistById working. This was my first time 
working on the patch function as in the weeks prior our groups would get stuck before we got to that.
I struggled for a bit before realising that I had to clearly write out the keys in the json object that 
I wanted to update. In this case it was just "name". So I had to define the parameter of the callback function
as const updates = {name} to refer to the sql statement where I am trying to change the name.

I am confident that I can easily translate this same code to the albums.js file. The only difference is that
I will include things like album date released. and album title in the const updates = {}, in addition to the 
sql statement where I will change not only the album title, but also date released.