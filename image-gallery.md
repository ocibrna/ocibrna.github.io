---
layout: post
permalink:
---

<html>
<head>
  <title>Image Gallery</title>
  <style>
    /* CSS for styling the gallery and modal */
    .gallery {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: center;
    }

    .gallery img {
      width: 250px;
      height: 200px;
      cursor: pointer;
    }

    .modal {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.7);
      justify-content: center;
      align-items: center;
    }

    .modal-content {
      max-width: 80%;
      max-height: 80%;
      margin: auto;
    }

    .modal-content img {
      max-width: 100%;
      max-height: 100%;
    }

    /* CSS for navigation arrows */
    .prev, .next {
      cursor: pointer;
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      font-size: 24px;
      font-weight: bold;
      padding: 10px;
      background-color: rgba(255, 255, 255, 0.7);
      border: 1px solid #ddd;
      border-radius: 5px;
      user-select: none;
    }

    .prev {
      left: 10px;
    }

    .next {
      right: 10px;
    }
  </style>
</head>
<body>
  <div class="gallery">
    
    <img src="/assets2/vystava/01IMG_3730.jpg" alt="Image 1" onclick="openModal('/assets2/vystava/01IMG_3730.jpg')" />
    <img src="/assets2/vystava/02IMG_3649.jpg" alt="Image 2" onclick="openModal('/assets2/vystava/02IMG_3649.jpg')" />
    <img src="/assets2/vystava/04IMG_3665.jpg" alt="Image 3" onclick="openModal('/assets2/vystava/04IMG_3665.jpg')" />
    <img src="/assets2/vystava/06IMG_3682.jpg" alt="Image 3" onclick="openModal('/assets2/vystava/06IMG_3682.jpg')" />
    <img src="/assets2/vystava/07IMG_3668.jpg" alt="Image 3" onclick="openModal('/assets2/vystava/07IMG_3668.jpg')" />
    <img src="/assets2/vystava/12IMG_3689.jpg" alt="Image 3" onclick="openModal('/assets2/vystava/12IMG_3689.jpg')" />
    <img src="/assets2/vystava/13IMG_3693.jpg" alt="Image 3" onclick="openModal('/assets2/vystava/13IMG_3693.jpg')" />
    <img src="/assets2/vystava/17IMG_3768.jpg" alt="Image 3" onclick="openModal('/assets2/vystava/17IMG_3768.jpg')" />             
    
  </div>

    <!-- The modal overlay -->
  <div id="myModal" class="modal">
    <span class="prev" onclick="changeImage(-1)">&#9665;</span>
    <div class="modal-content">
      <img id="modalImage" src="" alt="Enlarged Image" />
    </div>
    <span class="next" onclick="changeImage(1)">&#9655;</span>
  </div>

  <script>
    
    let currentImageIndex = 0;
    const imageUrls = ["/assets2/vystava/01IMG_3730.jpg", "/assets2/vystava/02IMG_3649.jpg", "/assets2/vystava/04IMG_3665.jpg", "/assets2/vystava/06IMG_3682.jpg", "/assets2/vystava/07IMG_3668.jpg", "/assets2/vystava/12IMG_3689.jpg", "/assets2/vystava/13IMG_3693.jpg", "/assets2/vystava/17IMG_3768.jpg"]; 
    const modalImage = document.getElementById('modalImage');

    function openModal(imageUrl) {
      const modal = document.getElementById('myModal');
      currentImageIndex = imageUrls.indexOf(imageUrl);
      modalImage.src = imageUrl;
      modal.style.display = 'flex';
    }

    function closeModal() {
      const modal = document.getElementById('myModal');
      modal.style.display = 'none';
    }

    function changeImage(step) {
      currentImageIndex += step;

      if (currentImageIndex < 0) {
        currentImageIndex = imageUrls.length - 1;
      } else if (currentImageIndex >= imageUrls.length) {
        currentImageIndex = 0;
      }

      modalImage.src = imageUrls[currentImageIndex];
    }

    // Close the modal when clicking outside the image
    window.onclick = function(event) {
      const modal = document.getElementById('myModal');
      if (event.target === modal) {
        closeModal();
      }
    };
  </script>
</body>
</html>