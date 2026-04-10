# html-javascript-bootcamp

Fork this repository to your GitHub account.

## Tasks

### Task 1  
Fix all HTML and JavaScript errors in files *broken-greeting.html* and *broken-greeting.js* (at least 8), rename them to *fixed-greeting.html* and *fixed-greeting.js*. 

Make the page work correctly so that:

- The JavaScript file is linked properly from the HTML.
- The button responds to a click.
- The input value is read correctly.
- The output message appears inside the correct element on the page.

#### Brief

- Correct the `<script>` tag so it points to the right file.
- Make sure the HTML `id` values match the ones used in JavaScript.
- Fix any missing brackets, braces, or semicolons.
- Fix any misspelled JavaScript methods or function names.
- Use `textContent` (or `innerText`) to update the output paragraph with a clear message.
- Test the page: type a name, click the button, check the result.

---

### Task 2  
Mini project – interactive page

Create a simple interactive page called *mini.html* with an external file *mini.css* and a JavaScript file *mini.js*.

You can choose one of these ideas (or a similar one):

- Favourite colour app (type a colour, show it in a sentence)
- Score checker (type a score, show “Pass” or “Try again”)
- Yes/No quiz checker (type an answer, show if it is correct)

#### Brief

- Create a semantic page using at least: `header`, `main`, and `footer`.
- Add a clear heading for your app.
- Add at least one `<input>` and one `<button>`.
- Use JavaScript to respond when the button is clicked.
- Show the result in a paragraph or box on the page.
- Link both your CSS file and your JavaScript file.
- Use margin and padding so the page looks neat and easy to read.

#### Starter HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Favourite Colour App</title>
  <link rel="stylesheet" href="mini.css" />
</head>
<body>
  <header>
    <h1>Favourite Colour App</h1>
    <p>Type your favourite colour and click the button.</p>
  </header>

  <main>
    <section>
      <input type="text" id="colourInput" placeholder="Enter a colour" />
      <button id="showBtn">Show Result</button>
      <p id="result"></p>
    </section>
  </main>

  <footer>
    <p>Created for JavaScript practice.</p>
  </footer>

  <script src="mini.js"></script>
</body>
</html>
```

#### Starter CSS

```css
body {
  font-family: Arial, sans-serif;
  margin: 0;
  background: #f4f4f4;
  color: #222;
}

header,
footer {
  background: #0f5f79;
  color: white;
  padding: 20px;
}

main {
  padding: 20px;
}

section {
  background: white;
  border: 1px solid #ddd;
  margin-bottom: 16px;
  padding: 16px;
}

h1 {
  margin-top: 0;
}

input,
button {
  padding: 10px;
  margin-right: 8px;
}

#result {
  margin-top: 16px;
  font-weight: bold;
}
```

#### Starter JavaScript

```javascript
let showBtn = document.getElementById("showBtn");
let colourInput = document.getElementById("colourInput");
let result = document.getElementById("result");

showBtn.addEventListener("click", function () {
  let colour = colourInput.value;

  if (colour === "") {
    result.textContent = "Please type a colour first.";
  } else {
    result.textContent = "Your favourite colour is " + colour + ".";
  }
});
```

### Task 3  
Publish your mini project to GitHub Pages

Take your finished mini project from Task 2 and publish it online using GitHub Pages.

#### Brief

- Make sure your project files are saved in your GitHub repository.
- Your main page should be called `index.html` if you want it to open automatically on GitHub Pages (otherwise, README.MD opens by default).
- Open your repository on GitHub.
- Go to **Settings**.
- Click **Pages** in the left menu.
- Under **Build and deployment**, choose:
  - **Source:** Deploy from a branch
  - **Branch:** `main`
  - **Folder:** `/root`
- Click **Save**.
- Wait a minute for GitHub Pages to publish your site.
- Open the live link and test that your project works online.

#### Files to include

- `index.html`
- `mini.css`
- `mini.js`

If your main file is currently called `mini.html`, rename it to `index.html` before publishing.

---

#### Submission checklist

- I linked my JavaScript file correctly in the HTML.
- I fixed the broken greeting app so the button works.
- I used the correct IDs in both HTML and JavaScript.
- I used a click event (or another suitable event) to run my code.
- I updated the page output using `textContent` or similar.
- I tested my code after making changes.
- I submitted a working editor link or zip file.
- I created a separate mini project page that responds to user input.
- I renamed my main page to `index.html`.
- I enabled GitHub Pages in the repository settings.
- I opened my live GitHub Pages link.
- I tested that the button and JavaScript still work online.
- I submitted my GitHub Pages URL.
