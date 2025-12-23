# Ex.07 Design of Interactive Image Gallery
## Date:23.12.2025

## AIM:
To design a web application for an inteactive image gallery for a minimum five images with next and previous buttons.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM:
```
gallery.html

<html>
<head>
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1>Interactive Image Gallery</h1>

    <div class="gallery-container">
        <img id="galleryImage" src="image1.png" alt="Gallery Image">

        <div class="buttons">
            <button id="prevBtn">Previous</button>
            <button id="nextBtn">Next</button>
        </div>
    </div>


    <footer>
        <p>Designed & Developed by G.devendran © 2025</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

style.css

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    text-align: center;
}

h1 {
    margin-top: 20px;
}

.gallery-container {
    width: 500px;
    margin: 30px auto;
    background: white;
    padding: 15px;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0,0,0,0.2);
}

.gallery-container img {
    width: 100%;
    height: 300px;
    object-fit: cover;
    border-radius: 5px;
}

.buttons {
    margin-top: 15px;
}

button {
    padding: 10px 20px;
    font-size: 16px;
    margin: 5px;
    border: none;
    border-radius: 5px;
    background-color: #007bff;
    color: white;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
}
footer {
    margin-top: auto;
    background-color: #333;
    color: white;
    padding: 15px 0;
    font-size: 14px;
}

script.js

const images = [
    "image2.png",
    "image3.png",
    "image4.png",
    "image5.png",
    "image6.png"
];

let currentIndex = 0;

const galleryImage = document.getElementById("galleryImage");
const nextBtn = document.getElementById("nextBtn");
const prevBtn = document.getElementById("prevBtn");

nextBtn.addEventListener("click", () => {
    currentIndex = (currentIndex + 1) % images.length;
    galleryImage.src = images[currentIndex];
});

prevBtn.addEventListener("click", () => {
    currentIndex = (currentIndex - 1 + images.length) % images.length;
    galleryImage.src = images[currentIndex];
});


```

## OUTPUT:
![alt text](<Screenshot (37).png>)
![alt text](<Screenshot (32).png>)
![alt text](<Screenshot (33).png>) 
![alt text](<Screenshot (34).png>)
![alt text](<Screenshot (35).png>) 
![alt text](<Screenshot (36).png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
