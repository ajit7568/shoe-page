# shoe-page
https://ajit7568.github.io/shoe-page/
<!-- This is an HTML document -->
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Set the character encoding for the document -->
    <meta charset="UTF-8" />
    <!-- Specify the version of Internet Explorer to be used -->
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <!-- Configure the viewport settings for responsive design -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!-- Link to an external CSS file for styling -->
    <link rel="stylesheet" href="style.css">
    <!-- Set the title of the webpage (displayed in the browser tab) -->
    <title>Document</title>
</head>
<body oncontextmenu="return false;">
    <!-- Create a container div to hold the content -->
    <div class="container">
        <!-- Create a div for displaying information about a shoe -->
        <div class="shoe" style=" background: linear-gradient(to right, #8a2387, #e94057, #f27121);">
            <!-- Create a div for the shoe description -->
            <div class="des">
                <!-- Display the heading for the shoe -->
                <h1>Shoe-1</h1>
                <!-- Display the first paragraph of the shoe description -->
                <p>
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Amet at,
                    blanditiis saepe adipisci molestiae neque quisquam perferendis,
                    repudiandae repellendus odio a repellat minus iste sapiente
                    molestias nulla nam, quas perspiciatis!
                </p>
                <!-- Display the second paragraph of the shoe description -->
                <p>
                    Lorem ipsum Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Rem, dolore.
                </p>
            </div>
            <!-- Display an image of the shoe -->
            <img class="shoe-1" src="shoe-1.png" alt="shoe1" />
        </div>
    </div>
</body>
</html>
css code
/* Apply a CSS reset to reset margins, paddings, and box sizing for all elements */
   * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    }

/* Set the background color of the body */
body {
    background-color: lightgrey;
}

/* Create a container for the content */
.container {
    width: 100%;
    height: 100vh;
    position: relative;
    overflow: hidden;
}

/* Create a gradient background for the container */
.container::after {
    content: "";
    position: absolute;
    inset: 0;
    transform: skewY(10deg);
    background: linear-gradient(to right, #b92b27, #1565c0);
    z-index: -1;
    box-shadow: 0px 0px 10px black;
}

/* Style the main shoe container */
.shoe {
    width: 85%;
    height: 75%;
    padding: 2%;
    margin: auto;
    margin-top: 7.5%;
    box-shadow: 0px 0px 10px black;
}

/* Style the shoe description */
.des {
    max-width: 40%;
    color: white;
}

/* Style the heading in the shoe description */
.des > h1 {
    font-size: xx-large;
    margin-bottom: 30px;
}

/* Style the paragraphs in the shoe description */
.des > p {
    font-size: large;
    margin-bottom: 50px;
    line-height: 20px;
}

  /* Style the shoe image */
.shoe-1 {
    position: absolute;
    right: 0px;
    top: 10%;
    width: 600px;
    height: 300px;
}

/* Enlarge the shoe image on hover */
.shoe-1:hover {
    right: 0px;
    top: 15px;
    width: 900px;
    height: 600px;
}

