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
        <script>
            function openModal(imageSrc) {
                document.getElementById('modalImage').src = imageSrc;
                document.getElementById('modal').style.display = 'block';
                document.getElementById('modalBackdrop').style.display = 'block';
            }
            function closeModal() {
                document.getElementById('modal').style.display = 'none';
                document.getElementById('modalBackdrop').style.display = 'none';
            }
        </script>
       <style>
        body{
            background-image:url(feather.jpg) ;
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: cover;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            text-align: center;
            font-family: "Lucida Handwriting";
            text-size-adjust: 54;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            padding: 20px;
        }
        .gallery-item {
            width: 295px;
            border: 3px solid #0b0b0b;
            border-radius: 40px;
            overflow: hidden;
            text-align: center;
            cursor: pointer;
            transition: transform 0.2s;
        }
        .gallery-item:hover {
            transform: scale(1.1);
        }
        .gallery-item img {
            width: 100%;
            height: auto;
        }
        .modal {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: rgb(255, 255, 255);
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            z-index: 1000;
            text-align: center;
            width: 30%;
            height: 50%;
        }
        .modal img {
            max-width: 100%;
            max-height: 80vh;
        }
        .modal-backdrop {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.7);
            z-index: 999;
        }
    </style>
</head>
<body>
    <header>
        <br><br><h1><b>MY GALLERY</b></h1>
    </header>
    <div class="gallery">
        <div class="gallery-item" onclick="openModal('bird2.jpeg')">
            <img src="bird2.jpeg" alt="Image-1">
        </div>
        <div class="gallery-item" onclick="openModal('bird7.jpeg')">
            <img src="bird7.jpeg" alt="Image-2">
        </div>
        <div class="gallery-item" onclick="openModal('bird6.jpeg')">
            <img src="bird6.jpeg" alt="Image-3">
        </div>
        <div class="gallery-item" onclick="openModal('bird5.jpeg')">
            <img src="bird5.jpeg" alt="Image-4">
        </div>
        <div class="gallery-item" onclick="openModal('bird4.jpeg')">
            <img src="bird4.jpeg" alt="Image-5">
        </div>
        <div class="gallery-item" onclick="openModal('bird3.jpeg')">
            <img src="bird3.jpeg" alt="Image-6">
        </div>
        <div class="gallery-item" onclick="openModal('bird10.jpeg')">
            <img src="bird10.jpeg" alt="Image-7">
        </div>
        <div class="gallery-item" onclick="openModal('bird1.jpeg')">
            <img src="bird1.jpeg" alt="Image-8">
        </div>
    </div>
    <div class="modal-backdrop" id="modalBackdrop" onclick="closeModal()"></div>
    <div class="modal" id="modal">
        <img id="modalImage" src="" alt="Expanded Image" width="100%" height="100%">
    </div>
    </body>
</html>
```

## OUTPUT
Screenshot 2025-05-09 124315.png
Screenshot 2025-05-09 124330.png
Screenshot 2025-05-09 124344.png
Screenshot 2025-05-09 124404.png
## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
