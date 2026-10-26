## Assignment 5.5 — CSS Fundamentals Mini-Project

### 1. `style.css`

```css
:root {
    --primary: #123c69;
    --secondary: #f0f4f8;
    --text: #333;
    --spacing: 16px;
}

* {
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: var(--secondary);
    color: var(--text);
    margin: 0;
    line-height: 1.6;
}

nav {
    background: var(--primary);
    padding: var(--spacing);
}

nav a {
    color: white;
    text-decoration: none;
    margin-right: 20px;
}

nav a:hover {
    color: #ffd700;
}

h1, h2 {
    color: var(--primary);
}

p {
    font-size: 16px;
}

button {
    background: var(--primary);
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

input, select {
    display: block;
    width: 100%;
    max-width: 400px;
    padding: 10px;
    margin: 10px 0;
}

table {
    width: 100%;
    border-collapse: collapse;
    background: white;
}

th, td {
    border: 1px solid #ccc;
    padding: 12px;
    text-align: left;
}

th {
    background: var(--primary);
    color: white;
}

.card {
    background: white;
    padding: var(--spacing);
    margin: var(--spacing) 0;
    border-radius: 8px;
}
```

### 2. Link CSS in All HTML Pages

Add this inside the `<head>` section of `index.html`, `about.html`, `registration.html`, and `contact.html`:

```html
<link rel="stylesheet" href="style.css">
```

### 3. Design Explanation

1. External CSS keeps the design separate from HTML.
2. Navy blue and light grey provide a consistent color palette.
3. Arial font improves readability.
4. CSS variables make colors and spacing reusable.
5. Chrome DevTools (`F12`) helps inspect and debug styling issues.

**Submission:** Submit all four HTML pages and `style.css`. Test every page using Live Server.