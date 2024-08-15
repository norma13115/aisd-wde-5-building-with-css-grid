
# WDE05 Building with CSS Grid

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

   **Explanation:** These two files are the core components of your project. `index.html` is where you'll write the structure and content of your webpage, while `styles.css` will contain all the styles that will be applied to the HTML elements. By separating HTML and CSS into different files, you follow a best practice that makes your code easier to maintain and update.

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

   **Explanation:** The HTML boilerplate is a standard structure that forms the foundation of any HTML document. It includes:

   - `<!DOCTYPE html>`: Declares the document type and version of HTML.
   - `<html lang="en">`: The root element of the HTML page, with a `lang` attribute specifying the language.
   - `<head>`: Contains meta-information about the document, including the character set, viewport settings for responsive design, and the title of the page.
   - `<link rel="stylesheet" href="styles.css" />`: Links the external CSS file to the HTML document, allowing the styles defined in `styles.css` to be applied.
   - `<body>`: The container for all the visible content on the page.

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

   **Explanation:** This block of HTML defines the main content of your page:

   - `<h2>Basic Concepts of Grid Layout</h2>`: A heading that introduces the section of the page.
   - `<div class="grid-container">`: A `div` element with the class `grid-container` that will serve as the parent container for the grid layout.
   - Inside the grid container, there are six `div` elements with the class `box` and unique classes (`box1`, `box2`, etc.). These `div`s represent the grid items that will be styled and positioned using CSS Grid.

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

   **Explanation:** This CSS provides the initial styling for your page:

   - The `body` selector applies global styles to the entire page, including font settings, margin and padding resets, flexbox properties for centering content, and a background color.
   - The `h1` selector styles the main heading, adjusting its margins, font size, and color to enhance readability and aesthetics.

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

   **Explanation:**

   - `.grid-container`: This class defines a grid container, transforming the `div` into a flexible grid layout. The `grid-template-columns` property uses the `repeat()` function to create responsive columns that automatically adjust based on available space. The `gap` property adds space between grid items, and the `padding`, `max-width`, and `width` properties control the overall size and spacing of the grid container.
   - `.box`: This class is applied to each grid item, ensuring they are displayed with centered content. The `display: flex;` property is used to align and justify the content within each box, making sure it appears centered. The boxes have a fixed height, a bold font, white text color, and a border with rounded corners for a polished appearance.

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

   **Explanation:**

   - These CSS classes (`.box1`, `.box2`, etc.) apply distinct background colors to each of the boxes within the grid. The colors are chosen to make each box stand out, enhancing the visual appeal and making it easy to distinguish between different grid items.

7. **Testing Your Layout:**
   - Resize the browser window to see how the grid adapts to different screen sizes.
   - Copy and paste the HTML boxes a few more times to see the grid expand and wrap into the next line. Resize the window to see the grid automatically resize.

   **Explanation:**

   - This step is crucial for testing the responsiveness of your grid layout. By resizing the browser window and adding more boxes, you can observe how the grid behaves across different screen sizes, ensuring that the layout remains consistent and functional on any device.

## AI Assistance

If you have any questions or need further explanations, feel free to ask the AI for help. Here are some examples of what you might ask:

- "How do I create a grid layout with CSS Grid?"
- "How can I ensure my layout is responsive?"

Good luck, and have fun building with the grid!

---

© All rights reserved to ThriveDX
