# Ex.07 Design of Interactive Image Gallery
## Date:09.05.25

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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="gallery.css">
</head>
<body>
    <div class="gallery-container">
        <div class="gallery-item">
            <img src="1.jpg" alt="Image 1">
        </div>
        <div class="gallery-item">
            <img src="2.jpg" alt="Image 2">
        </div>
        <div class="gallery-item">
            <img src="3.jpg" alt="Image 3">
        </div>
        <div class="gallery-item">
            <img src="4.jpg" alt="Image 4">
        </div>
        <div class="gallery-item">
            <img src="5.jpg" alt="Image 5">
        </div>
    </div>

    <div class="modal" id="modal">
        <span class="close" id="close">&times;</span>
        <img class="modal-content" id="modal-img">
    </div>

    <script src="gallery.js"></script>
</body>
</html>
 /* Body Styling */
body {
    margin: 0;
    padding: 0;
    background-color: #e3e0e0;
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    overflow: hidden;
}

/* Gallery Container */
.gallery-container {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 15px;
    padding: 20px;
    max-width: 1200px;
    width: 100%;
}

/* Individual Image Items */
.gallery-item img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease-in-out;
}

.gallery-item img:hover {
    transform: scale(1.2);
    cursor: pointer;
}

/* Modal Background */
.modal {
    display: none;
    position: fixed;
    z-index: 10;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    overflow: auto;
    background-color: rgba(0, 0, 0, 0.7);
}

/* Modal Image */
.modal-content {
    display: block;
    margin: 60px auto;
    max-width: 700px;
    width: 80%;
    border-radius: 10px;
    animation: zoomIn 0.3s ease;
}

/* Close Button */
.close {
    position: absolute;
    top: 30px;
    right: 40px;
    font-size: 35px;
    font-weight: bold;
    color: #fff;
    cursor: pointer;
}

.close:hover {
    color: #bbb;
}

/* Animation */
@keyframes zoomIn {
    from {
        transform: scale(0.5);
        opacity: 0;
    }
    to {
        transform: scale(1);
        opacity: 1;
    }
}



```
## OUTPUT:
![image](https://github.com/user-attachments/assets/0d34b5d5-e88e-48c9-99f2-570b08f8a0da)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
