# Ex.08 Design of Interactive Image Gallery
## Date:12.10.25

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

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

## PROGRAM :
```
index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Nature's Gallery</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <script src="script.js"></script>
</body>
</html>

style.css
body {
  font-family: Arial, sans-serif;
  background-color: #a19797;
  margin: 0;
  padding: 0;
  text-align: center;
}

h2, h3 {
  color: #ebf5ef;
  margin-top: 20px;
}

.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 15px;
  padding: 20px;
  max-width: 1200px;
  margin: auto;
}

.gallery img {
  width: 100%;
  height: 250px;
  object-fit: cover;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.2);
  transition: transform 0.3s;
}

.gallery img:hover {
  transform: scale(1.05);
}

script.js
const heading1 = document.createElement("h2");
heading1.textContent = "JOSHUA DANIEL A (25017654)";
document.body.appendChild(heading1);

const heading2 = document.createElement("h3");
heading2.textContent = "Nature's Gallery";
document.body.appendChild(heading2);
const gallery = document.createElement("div");
gallery.className = "gallery";
document.body.appendChild(gallery);
const images = [
  { src: "r.jpeg", alt: "River" },
  { src: "b.jpeg", alt: "Beach" },
  { src: "m.jpg", alt: "Joshua Daniel A" },
  { src: "d.jpeg", alt: "Desert" },
  { src: "w.jpeg", alt: "Waterfall" }
];
images.forEach(imgData => {
  const img = document.createElement("img");
  img.src = imgData.src;
  img.alt = imgData.alt;
  gallery.appendChild(img);
});
```

## OUTPUT:
![alt text](<Screenshot (84).png>)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
