# Practical-13-Pseudo-classes-and-Pseudo-elements

<!DOCTYPE html>
<html>
<head>
    <title>Pseudo Selectors</title>
    <style>
        body {
            font-family: Arial;
        }

        a {
            display: inline-block;
            padding: 10px;
            background: lightblue;
        }

        a:hover {
            background: yellow;
        }

        a:focus {
            outline: 2px solid blue;
        }

        a:active {
            background: red;
            color: white;
        }

        li:nth-child(even) {
            color: blue;
        }

        h2::before {
            content: "★ ";
            color: orange;
        }

        h2::after {
            content: " ★";
            color: orange;
        }

        p::first-letter {
            font-size: 35px;
            color: red;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h2>Interactive Menu</h2>

    <a href="#article">Home</a>
    <a href="#article">About</a>
    <a href="#article">Contact</a>

    <h2>Menu Items</h2>
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
        <li>Python</li>
    </ul>

    <h2 id="article">Article</h2>
    <p>CSS is used to style web pages.
       It controls colors, layouts, fonts and spacing.</p>
</body>
</html>
