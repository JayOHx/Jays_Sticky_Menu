# Information:

This is a simple HTML based sticky menu for website use. Currently it hosts the beggings of a CSGO gambling site but can be easily changed to fit any purpose. It uncludes a small amount of CSS than could be added to the HTML file if you wish but I just like to keep things tidy, also a very small amount of JS to control what the menu does and when.

# Support:

I will not be providing support for this as I am only just entering the world of HTML as I am trying to expand my knwowledge.

# How to use:
1. Change the file paths in each of the .html files, there is 5 paths in each file that need changing.
2. Ensure you're pages match, for example, ensure that you're 'home' path links to the actual homepage.html in all 5 files.
3. Do the same for the other 4 paths to the other pages in all files.
4. Finally, update how you like by changing colors or what ever else.

#Example:

a class="active" href="YOUR_NEW_FILE_PATH">Home</a

-- Don't forget to include < and > at each end of this line above otherwise it won't work.

# Test

<!doctype html>

<title>CSGOPhoenix.com - Home</title>
<link rel="shortcut icon" href="/favicon.ico"/>

<html>
  <body>

  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="style.css">

  <div id="navbar">
    <a class="active" href="file:///C:/Users/Jay%20O'Halloran/Desktop/html/homepage.html">Home</a>
    <a href="file:///C:/Users/Jay%20O'Halloran/Desktop/html/crash.html">Crash</a>
    <a href="file:///C:/Users/Jay%20O'Halloran/Desktop/html/roulette.html">Roulette</a>
    <a href="file:///C:/Users/Jay%20O'Halloran/Desktop/html/dice.html">Dice</a>
    <a href="file:///C:/Users/Jay%20O'Halloran/Desktop/html/plinko.html">Plinko</a>
  </div>

  <script>
  window.onscroll = function() {myFunction()};

  var navbar = document.getElementById("navbar");
  var sticky = navbar.offsetTop;

  function myFunction() {
    if (window.pageYOffset >= sticky) {
      navbar.classList.add("sticky")
    } else {
      navbar.classList.remove("sticky");
    }
  }
  </script>

</body>
</html>






