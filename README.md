# Building with CSS Grid
![Screenshot of the project](assets/images/example.png)

## Description
This assignment will help you create a responsive layout using CSS Grid. You'll learn how to set up your HTML and CSS files, include the necessary boilerplate code, and add CSS Grid code step-by-step.

## Prerequisites

- Basic knowledge of HTML and CSS

## Project Structure

```
grid_layout_project
│   index.html
│   styles.css
```

## Steps

1. **Create HTML and CSS Files:**

   - Create a new HTML file named `index.html`.
   - Create a new CSS file named `styles.css`.

2. **Add Boilerplate Code to HTML:**

   - Open `index.html` and add the following boilerplate code:

   ```html
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="UTF-8" />
       <meta name="viewport" content="width=device-width, initial-scale=1.0" />
       <title>Basic Concepts of Grid Layout</title>
       <link rel="stylesheet" href="styles.css" />
     </head>
     <body>
       <!-- Your Grid Div Code Goes Here  -->
     </body>
   </html>
   ```

3. **Add Body Content to HTML:**

   - In `index.html` between the `<body>` tags, add the following content:

   ```html
       <h2>Basic Concepts of Grid Layout</h2>
       <div class="grid-container">
           <div class="box box1">Box 1</div>
           <div class="box box2">Box 2</div>
           <div class="box box3">Box 3</div>
           <div class="box box4">Box 4</div>
           <div class="box box5">Box 5</div>
           <div class="box box6">Box 6</div>
       </div>
   ```

4. **Basic Styling:**

   - Open `styles.css` and add the following code:

   ```css
   body {
     font-family: Arial, sans-serif;
     margin: 0;
     padding: 0;
     display: flex;
     flex-direction: column;
     align-items: center;
     min-height: 100vh;
     background-color: #f0f0f0;
   }

   h1 {
     margin-top: 20px;
     margin-bottom: 20px;
     font-size: 2rem;
     color: #333;
   }
   ```

5. **Setting Up the Grid Layout:**

   - Add the following CSS to `styles.css` to create a responsive grid layout:

   ```css
   .grid-container {
     display: grid; /* This defines a grid container */
     grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Creates responsive columns that fit the available space */
     gap: 10px; /* Adds a 10px gap between grid items */
     padding: 10px;
     max-width: 1000px;
     width: 100%;
   }

   .box {
     display: flex;
     justify-content: center;
     align-items: center;
     height: 150px;
     color: white;
     font-size: 1.2rem;
     font-weight: bold;
     text-align: center;
     border: 2px solid #000;
     border-radius: 8px;
   }
   ```

6. **Adding Colors to the Boxes:**

   - Add the following CSS to `styles.css` to style the individual boxes:

   ```css
   .box1 {
     background-color: #ff5733;
   } /* Red-Orange */
   .box2 {
     background-color: #33ff57;
   } /* Green */
   .box3 {
     background-color: #3357ff;
   } /* Blue */
   .box4 {
     background-color: #f3ff33;
   } /* Yellow */
   .box5 {
     background-color: #ff33a1;
   } /* Pink */
   .box6 {
     background-color: #33fff5;
   } /* Cyan */
   ```

7. **Testing Your Layout:**
   - Resize the browser window to see how the grid adapts to different screen sizes.
   - Copy and paste the HTML boxes a few more times to see the grid expand and wrap into the next line. Resize the window to see the grid automatically resize.

## AI Assistance

If you have any questions or need further explanations, feel free to ask the AI for help. Here are some examples of what you might ask:

- "How do I create a grid layout with CSS Grid?"
- "How can I ensure my layout is responsive?"

Good luck, and have fun building with the grid!
