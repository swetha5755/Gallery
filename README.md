# Ex.08 Design of Interactive Image Gallery
# Date:16.12.2024
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PHOTO DUMP</title>
    <style>
        body {
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-image: url(https://i.pinimg.com/736x/be/f4/e5/bef4e592e6dabb18e2ae22301e8fc95d.jpg);
            background-size: cover;  
            background-position: center;   
        }

        h1 {
            margin-top: 20px;
            font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            padding: 20px;
        }

        .gallery img {
            width: 200px;
            height: 150px;
            border: 6px solid #000000;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid rgb(1, 1, 1);
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1><u>PHOTO DUMP</u></h1>
    <div class="gallery">
        <img src=https://i.pinimg.com/736x/ee/c0/6b/eec06bcaf01f283d92ff48c9ad3f7407.jpg alt="Image 1" onclick="openModal(this)">
        <img src=https://i.pinimg.com/736x/32/2f/51/322f51600dbd9d4a6743f1687c083235.jpg alt="Image 2" onclick="openModal(this)">
        <img src=https://i.pinimg.com/736x/fe/40/cb/fe40cb0da3bf1f778088081faecb7051.jpg alt="Image 3" onclick="openModal(this)">
        <img src=https://i.pinimg.com/736x/08/3b/4b/083b4b0b06d216c06b995c95cbe6bd8d.jpg alt="Image 4" onclick="openModal(this)">
        <img src=https://i.pinimg.com/736x/a7/b8/26/a7b826101627454b6e1ba2b900559c80.jpg alt="Image 5" onclick="openModal(this)">
        <img src=https://i.pinimg.com/736x/cd/39/39/cd3939f55a612b0dfa97515f137bade5.jpg alt="Image 1" onclick="openModal(this)">
        <img src=https://i.pinimg.com/736x/54/83/0d/54830dd932312c2a224334b553d97e77.jpg alt="Image 2" onclick="openModal(this)">
        <img src=https://i.pinimg.com/736x/8a/d3/bb/8ad3bb25e474aaa3332d183b750fe7ff.jpg alt="Image 3" onclick="openModal(this)">
        <img src=https://i.pinimg.com/736x/4b/9c/0a/4b9c0a8f21b94c152ac14484cf5f2636.jpg alt="Image 4" onclick="openModal(this)">
        <img src=https://i.pinimg.com/736x/a7/da/a9/a7daa96861c7c881ee2da7edea483eb0.jpg alt="Image 5" onclick="openModal(this)">
    </div>

    <!-- Modal for displaying larger image -->
    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <script>
        // Function to open the modal and display the clicked image
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }

        // Function to close the modal
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>
</body>
</html>
```
# OUTPUT:
![Screenshot 2024-12-16 003053](https://github.com/user-attachments/assets/1b711130-6efb-436e-b7f4-d5426ab0cef8)
![Screenshot 2024-12-16 003119](https://github.com/user-attachments/assets/abef34e5-77ad-42a6-b76b-fd3d9c45652b)
# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
