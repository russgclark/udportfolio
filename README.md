## Website Performance Optimization portfolio project

Instructions
-----

Load index.html to view home page.  Pizza.html is accessible via the "Cam's Pizzeria" text link on the home page, or via the following path /views/pizza.html.

-----
index.html
-----

 - Added style.css content to head area to remove one http request

 - Added media="print" distinction to print.css link, allowing it to only be loaded when necessary

 - Added "async" tag to Google Analytics link, so that it does not cause a delay in rendering

 - Re-sized pizzeria thumbnail and compressed both it and profilepic.jpg via https://tinypng.com/

-----
pizza.html / main.js
-----

 - Re-sized pizzeria.jpg

 - Adjusted function changePizzaSizes on line 451 of main.js, placing variable assignments and selector usage outside loop, directly above it but still within function.  Loop now processes all re-sizable pizzas without having to repeat the same process multiple times within each run.

 - Adjusted function updatePositions on line 503 of main.js, placing the scrollTop calculation outside of the loop and assigning its value to a variable.  This allows the loop to avoid having to make an inefficient check each time it runs.
