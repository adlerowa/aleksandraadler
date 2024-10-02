---
layout: home
title: Welcome
---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hamburger Menu</title>
  <style>
    /* CSS for Hamburger Menu */
    .menu {
      display: none;
      flex-direction: column;
      background-color: #333;
      position: absolute;
      top: 50px;
      right: 0;
      width: 200px;
    }

    .menu a {
      color: white;
      padding: 10px;
      text-decoration: none;
      text-align: center;
    }

    .menu a:hover {
      background-color: #575757;
    }

    .hamburger {
      display: flex;
      flex-direction: column;
      cursor: pointer;
      width: 30px;
      height: 30px;
      justify-content: space-around;
    }

    .bar {
      width: 100%;
      height: 4px;
      background-color: black;
    }

    @media (min-width: 768px) {
      .menu {
        display: flex;
        flex-direction: row;
        position: static;
        width: auto;
      }

      .hamburger {
        display: none;
      }
    }
  </style>
</head>
<body>
  <div class="hamburger" onclick="toggleMenu()">
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
  </div>
  <div class="menu" id="menu">
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </div>

  <script>
    // JavaScript for toggling the menu
    function toggleMenu() {
      var menu = document.getElementById('menu');
      if (menu.style.display === 'flex') {
        menu.style.display = 'none';
      } else {
        menu.style.display = 'flex';
      }
    }
  </script>
</body>
</html>
# Hi! I'm Aleksandra Adler

I am a postdoctoral researcher in the cognitive neuroscience of language at Stockholm University.
Welcome to my personal website.


<div style="text-align: center; width: 100%;">
  <img src="adler_tolk.jpg" alt="My Photo" width="300" height="400">
</div>
