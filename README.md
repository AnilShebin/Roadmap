#### Day 1: March 14 - Welcome Banner
- **Task**: Create `day1.html` with a styled header, image, and button that reveals a welcome message.
- **Output**: A bold banner with an image and interactive greeting.
- **Code**:
  ```html
  <html>
  <head><style>h1 { color: white; background-color: navy; padding: 20px; text-align: center; } img { width: 200px; display: block; margin: 10px auto; } p { display: none; font-size: 18px; text-align: center; }</style></head>
  <body>
    <h1>Welcome!</h1>
    <img src="https://via.placeholder.com/200" alt="Banner">
    <button>Show Message</button>
    <p>Glad you're here!</p>
    <script>document.querySelector("button").onclick = function() { document.querySelector("p").style.display = "block"; };</script>
  </body>
  </html>
  ```
- **Resources**:
  1. [W3Schools: HTML Headings](https://www.w3schools.com/html/html_headings.asp) - Header basics.
  2. [MDN: CSS Display](https://developer.mozilla.org/en-US/docs/Web/CSS/display) - Show/hide styling.
  3. [W3Schools: JS Events](https://www.w3schools.com/js/js_events.asp) - Button interaction.

#### Day 2: March 15 - Profile Card
- **Task**: Create `day2.html` with a card (name, bio, image), styled with a border, and a button to toggle the bio.
- **Output**: A personal profile card with a toggle feature.
- **Code**:
  ```html
  <html>
  <head><style>.card { border: 2px solid gray; width: 300px; margin: 20px auto; padding: 15px; text-align: center; } h2 { color: teal; } img { width: 100px; } p { font-size: 16px; }</style></head>
  <body>
    <div class="card">
      <h2>Your Name</h2>
      <img src="https://via.placeholder.com/100" alt="Profile">
      <p>I like coding!</p>
      <button>Toggle Bio</button>
    </div>
    <script>document.querySelector("button").onclick = function() { let p = document.querySelector("p"); p.style.display = p.style.display === "none" ? "block" : "none"; };</script>
  </body>
  </html>
  ```
- **Resources**:
  1. [W3Schools: HTML Div](https://www.w3schools.com/tags/tag_div.asp) - Container basics.
  2. [MDN: CSS Borders](https://developer.mozilla.org/en-US/docs/Web/CSS/border) - Card styling.
  3. [MDN: JS Toggle](https://developer.mozilla.org/en-US/docs/Web/API/Element/style) - Toggle logic.

#### Day 3: March 16 - Photo Gallery
- **Task**: Create `day3.html` with 3 images in a row, styled with borders, and a button to hide/show all.
- **Output**: A mini gallery with toggle functionality.
- **Code**:
  ```html
  <html>
  <head><style>.gallery { text-align: center; } img { width: 120px; margin: 10px; border: 2px solid black; } button { display: block; margin: 10px auto; padding: 5px; }</style></head>
  <body>
    <div class="gallery">
      <img src="https://via.placeholder.com/120" alt="Pic 1">
      <img src="https://via.placeholder.com/120" alt="Pic 2">
      <img src="https://via.placeholder.com/120" alt="Pic 3">
    </div>
    <button>Toggle Photos</button>
    <script>document.querySelector("button").onclick = function() { let imgs = document.querySelectorAll("img"); imgs.forEach(img => img.style.display = img.style.display === "none" ? "inline" : "none"); };</script>
  </body>
  </html>
  ```
- **Resources**:
  1. [W3Schools: HTML Images](https://www.w3schools.com/html/html_images.asp) - Image setup.
  2. [MDN: CSS Margin](https://developer.mozilla.org/en-US/docs/Web/CSS/margin) - Layout styling.
  3. [W3Schools: querySelectorAll](https://www.w3schools.com/jsref/met_document_queryselectorall.asp) - Multi-element control.

#### Day 4: March 17 - To-Do List
- **Task**: Create `day4.html` with an input, button, and `<ul>`, styled with colors, add JS to append tasks from input.
- **Output**: A functional to-do list with user input.
- **Code**:
  ```html
  <html>
  <head><style>h1 { color: darkgreen; text-align: center; } input { padding: 5px; margin: 10px; } button { background-color: green; color: white; padding: 5px; } ul { list-style-type: square; margin-left: 40px; }</style></head>
  <body>
    <h1>To-Do List</h1>
    <input type="text" placeholder="Add a task">
    <button>Add</button>
    <ul id="tasks"></ul>
    <script>document.querySelector("button").onclick = function() { let task = document.querySelector("input").value; document.querySelector("#tasks").innerHTML += "<li>" + task + "</li>"; };</script>
  </body>
  </html>
  ```
- **Resources**:
  1. [W3Schools: HTML Forms](https://www.w3schools.com/html/html_forms.asp) - Input basics.
  2. [MDN: List Style](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-type) - List styling.
  3. [W3Schools: JS Input](https://www.w3schools.com/jsref/prop_text_value.asp) - Input handling.

#### Day 5: March 18 - Weather Card
- **Task**: Create `day5.html` with a weather display (temp, condition), styled as a card, and a button to switch conditions.
- **Output**: A weather card that updates dynamically.
- **Code**:
  ```html
  <html>
  <head><style>.weather { width: 250px; margin: 20px auto; padding: 15px; background-color: lightblue; text-align: center; } h2 { color: navy; } p { font-size: 18px; }</style></head>
  <body>
    <div class="weather">
      <h2>Weather</h2>
      <p>25°C, Sunny</p>
      <button>Change</button>
    </div>
    <script>document.querySelector("button").onclick = function() { let p = document.querySelector("p"); p.innerText = p.innerText === "25°C, Sunny" ? "18°C, Rainy" : "25°C, Sunny"; };</script>
  </body>
  </html>
  ```
- **Resources**:
  1. [W3Schools: HTML Div](https://www.w3schools.com/tags/tag_div.asp) - Container recap.
  2. [MDN: Background Color](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color) - Card styling.
  3. [MDN: innerText](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/innerText) - Text switching.

#### Day 6: March 19 - Calculator Box
- **Task**: Create `day6.html` with two inputs and a result `<p>`, styled with borders, add a button to add the numbers.
- **Output**: A simple calculator for addition.
- **Code**:
  ```html
  <html>
  <head><style>.calc { width: 300px; margin: 20px auto; padding: 15px; border: 1px solid gray; } input { width: 80px; margin: 5px; } p { font-size: 20px; text-align: center; }</style></head>
  <body>
    <div class="calc">
      <input type="number" placeholder="Num 1">
      <input type="number" placeholder="Num 2">
      <button>Calculate</button>
      <p>Result: 0</p>
    </div>
    <script>document.querySelector("button").onclick = function() { let n1 = Number(document.querySelectorAll("input")[0].value); let n2 = Number(document.querySelectorAll("input")[1].value); document.querySelector("p").innerText = "Result: " + (n1 + n2); };</script>
  </body>
  </html>
  ```
- **Resources**:
  1. [W3Schools: HTML Input](https://www.w3schools.com/html/html_form_input_types.asp) - Number input.
  2. [MDN: CSS Width](https://developer.mozilla.org/en-US/docs/Web/CSS/width) - Sizing inputs.
  3. [W3Schools: JS Numbers](https://www.w3schools.com/js/js_numbers.asp) - Math operations.

#### Day 7: March 20 - Quote Generator
- **Task**: Create `day7.html` with a quote `<p>` and button, styled with a shadow, add JS to cycle through 3 quotes.
- **Output**: A quote box with random-like cycling.
- **Code**:
  ```html
  <html>
  <head><style>.quote { width: 400px; margin: 20px auto; padding: 20px; box-shadow: 2px 2px 5px gray; text-align: center; } p { font-size: 18px; } button { padding: 5px; background-color: orange; color: white; }</style></head>
  <body>
    <div class="quote">
      <p>"Dream big."</p>
      <button>Next Quote</button>
    </div>
    <script>let quotes = ["Dream big.", "Work hard.", "Stay positive."]; let i = 0; document.querySelector("button").onclick = function() { i = (i + 1) % 3; document.querySelector("p").innerText = '"' + quotes[i] + '"'; };</script>
  </body>
  </html>
  ```
- **Resources**:
  1. [W3Schools: HTML Paragraphs](https://www.w3schools.com/html/html_paragraphs.asp) - Text basics.
  2. [MDN: Box Shadow](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow) - Shadow styling.
  3. [MDN: Arrays](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) - Array cycling.

#### Day 8: March 21 - Memory Game
- **Task**: Create `day8.html` with 4 colored `<div>` boxes, styled in a grid, add JS to toggle their visibility on click.
- **Output**: A basic memory game layout with hide/show boxes.
- **Code**:
  ```html
  <html>
  <head><style>.game { width: 300px; margin: 20px auto; display: flex; flex-wrap: wrap; } .box { width: 60px; height: 60px; margin: 10px; cursor: pointer; } .red { background-color: red; } .blue { background-color: blue; } .green { background-color: green; } .yellow { background-color: yellow; }</style></head>
  <body>
    <div class="game">
      <div class="box red"></div>
      <div class="box blue"></div>
      <div class="box green"></div>
      <div class="box yellow"></div>
    </div>
    <script>document.querySelectorAll(".box").forEach(box => box.onclick = function() { this.style.display = this.style.display === "none" ? "block" : "none"; });</script>
  </body>
  </html>
  ```
- **Resources**:
  1. [W3Schools: HTML Div](https://www.w3schools.com/tags/tag_div.asp) - Box basics.
  2. [MDN: Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox) - Grid layout.
  3. [W3Schools: JS forEach](https://www.w3schools.com/jsref/jsref_foreach.asp) - Loop handling.

#### Day 9: March 22 - Event Countdown
- **Task**: Create `day9.html` with a countdown `<p>` (e.g., “5 days”), styled with a border, add a button to decrease it.
- **Output**: A countdown timer with a decrement feature.
- **Code**:
  ```html
  <html>
  <head><style>.countdown { width: 300px; margin: 20px auto; padding: 15px; border: 2px dashed purple; text-align: center; } h1 { color: darkred; } p { font-size: 20px; } button { padding: 5px; background-color: purple; color: white; }</style></head>
  <body>
    <div class="countdown">
      <h1>Event Countdown</h1>
      <p>5 days left</p>
      <button>Next Day</button>
    </div>
    <script>let days = 5; document.querySelector("button").onclick = function() { days--; document.querySelector("p").innerText = days + " days left"; if (days === 0) alert("Event is here!"); };</script>
  </body>
  </html>
  ```
- **Resources**:
  1. [W3Schools: HTML Headings](https://www.w3schools.com/html/html_headings.asp) - Title basics.
  2. [MDN: Border Style](https://developer.mozilla.org/en-US/docs/Web/CSS/border-style) - Dashed border.
  3. [MDN: JS if](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else) - Condition check.

#### Day 10: March 23 - Personal Dashboard
- **Task**: Create `day10.html` with a header, task input/list, and counter, styled with colors and layout, add JS for adding tasks and counting clicks.
- **Output**: A multi-feature dashboard for tasks and tracking.
- **Code**:
  ```html
  <html>
  <head><style>body { font-family: Arial; } h1 { color: white; background-color: darkblue; padding: 20px; text-align: center; } .dashboard { width: 400px; margin: 20px auto; } input { padding: 5px; width: 200px; } button { background-color: blue; color: white; padding: 5px; margin: 5px; } ul { margin: 10px 0; } p { font-size: 18px; text-align: center; }</style></head>
  <body>
    <h1>My Dashboard</h1>
    <div class="dashboard">
      <input type="text" placeholder="New Task">
      <button onclick="addTask()">Add Task</button>
      <ul id="tasks"></ul>
      <button onclick="countClick()">Click Me</button>
      <p>Clicks: 0</p>
    </div>
    <script>let clicks = 0; function addTask() { let task = document.querySelector("input").value; document.querySelector("#tasks").innerHTML += "<li>" + task + "</li>"; } function countClick() { clicks++; document.querySelector("p").innerText = "Clicks: " + clicks; }</script>
  </body>
  </html>
  ```
- **Resources**:
  1. [W3Schools: HTML Structure](https://www.w3schools.com/html/html_basic.asp) - Full page setup.
  2. [MDN: CSS Fonts](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family) - Font styling.
  3. [W3Schools: JS Functions](https://www.w3schools.com/js/js_functions.asp) - Function basics.

---

### Tips for Success
- **Setup**: Save each as `dayX.html`; copy-paste code into VS Code and test in browser.
- **Time**: Focus ~20 min on HTML, 20 min on CSS, 20 min on JS; tweak if needed.
- **Enhance**: Add your own colors, text, or features (e.g., clear tasks on Day 10).
- **Debug**: Use DevTools (F12) for CSS adjustments or JS errors.

### Why This Works
- **Bigger Projects**: Tasks like a calculator, memory game, and dashboard feel substantial.
- **Daily All-in-One**: HTML, CSS, JS in every project build well-rounded skills.
- **Practical**: Outputs are portfolio-ready and showcase real-world use.
