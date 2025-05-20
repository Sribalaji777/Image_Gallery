# Ex.08 Design of Interactive Image Gallery

## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
```
<html>
<head>
    <title>Album</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&family=Poppins:wght@600&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Poppins', sans-serif;
            background-image: url('BG.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            color: white;
            position: relative;
        }

        .overlay {
            background: rgba(244, 241, 241, 0.5);
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
        }

        header {
            text-align: center;
            padding: 20px;
            position: relative;
            z-index: 1;
        }

        h1 {
            color: #FF6347;
            font-size: 48px;
            margin: 10px 0;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
        }

        h2 {
            color: #7FFF00;
            font-size: 36px;
            margin: 10px 0;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin: 30px 0;
            position: relative;
            z-index: 1;
        }

        .gallery img {
            width: 230px;
            height: 230px;
            cursor: pointer;
            border-radius: 15px;
            border: 5px solid #52e8e3;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
        }

        footer {
            background-color: #FF4500;
            color: #fff;
            padding: 12px 30px;
            text-align: center;
            position: fixed;
            bottom: 0;
            width: 100%;
            z-index: 1;
        }

        .viewer {
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            position: fixed;
            top: 0;
            display: none;
            align-items: center;
            justify-content: center;
            z-index: 100;
        }

        .viewer img {
            width: 800px;
            height: auto;
            border: 5px solid #FFFFFF;
            border-radius: 10px;
        }

        .close-btn {
            color: #FF6347;
            position: absolute;
            top: 5%;
            right: 5%;
            font-size: 50px;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>

<body>
    <div class="overlay"></div>
    <header>
        <h1>My GALLERY</h1>
        <h2>7 WONDERS</h2>
    </header>

    <div class="gallery">
        <img src="taj mall.jpg" onclick="openViewer(this.src)" alt="Taj Mahal">
        <img src="kili.jpg" onclick="openViewer(this.src)" alt="Colosseum">
        <img src="pexels-palocech-286746.jpg" onclick="openViewer(this.src)" alt="Chichen Itza">
        <img src="china wall.jpg" onclick="openViewer(this.src)" alt="Great Wall of China">
        <img src="pexels-joao-ricardo-januzzi-94538344-9229056.jpg" onclick="openViewer(this.src)" alt="Cristo Redentor">
        <img src="pramit.jpg" onclick="openViewer(this.src)" alt="Machu Picchu">
        <img src="palaya.jpg" onclick="openViewer(this.src)" alt="Petra">
    </div>

    <div class="viewer" onclick="closeViewer()">
        <span class="close-btn" onclick="closeViewer()">&times;</span>
        <img src="" alt="Large view">
    </div>

    <footer>
        <p>Designed by sribalaji (24900249)</p>
    </footer>

    <script>
        function openViewer(src) {
            document.querySelector('.viewer img').src = src;
            document.querySelector('.viewer').style.display = 'flex';
        }

        function closeViewer() {0
            document.querySelector('.viewer').style.display = 'none';
        }
    </script>
</body>
</html>
```


## OUTPUT
![alt text](<Screenshot 2025-05-20 150730.png>)
![alt text](<Screenshot 2025-05-20 150747.png>)
![alt text](<Screenshot 2025-05-20 150805.png>)
![alt text](<Screenshot 2025-05-20 150828.png>)
![alt text](<Screenshot 2025-05-20 150849.png>)
![alt text](<Screenshot 2025-05-20 150909.png>)
![alt text](<Screenshot 2025-05-20 150922.png>)
![alt text](<Screenshot 2025-05-20 150936.png>)


## RESULT!
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
