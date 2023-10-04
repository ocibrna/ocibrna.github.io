---
layout: post
title: EXHIBIČNÍ SIMULTÁNNÍ ŠACHOVÁ PARTIE S JULIÍ A SERGEJEM MOVSESJANOVÝMI
---
---

<div class="ntext">
<p>
V pondělí 11. září 2023 ožila Moravská zemská knihovna mimořádnou šachovou událostí. Na prostranství před vstupem do budovy MZK se uskutečnila exhibiční simultánní šachová partie s velmistryní a přebornicí ČR Julií Movsesjanovou a arménským velmistrem, mistrem světa a olympijským vítězem Sergejem Movsesjanem. Akce byla zahájena v Konferenčním sále MZK představením velmistrů a výstavy o Eduardu Lendlovi. Mezi hosty nechyběl vnuk Eduarda Lendla, pan Karel Rybák. Poté už následovala simultánní partie před budovou. Julia a Sergej Movsesjanovi, kteří se střídali po jednom tahu, se společně utkali s 23 soupeři. 
</p>
<p>
Všechny partie zahájila šachová velmistryně. V kombinaci s klasickými soupravami mohlo hrát simultánku v jeden moment celkem 16 hráčů. Hned osm šachovnic bylo přenášeno online.
</p>
<p>
Po celou dobu akce probíhal souběžně v kavárně v MZK přenos exhibice s odborným komentářem Josefa Bednaříka a jeho hostů. Posluchači se dozvěděli zajímavosti ze života manželů Movsesjanových i hodnocení samotných partií ze šachové exhibice. 
</p>
<p>
Nejmladšímu účastníkovi bylo devět let a vydržel manželům Movsesjanovým vzdorovat hodinu a půl. Výborný výkon podal třináctiletý chlapec, který po třech hodinách uhrál s velmistry remízu. Konečný výsledek byly tři remízy, žádnému z účastníků se tentokrát zvítězit nepodařilo. 
</p>
<p>
Akcí chtěla MZK upozornit na právě probíhající výstavu Oči Brna: Eduard Lendl, která představuje zakladatele jedné z největších sbírek šachové literatury v Evropě! Její fond, jenž spravuje a dále rozvíjí Moravská zemská knihovna, dnes čítá na 6000 publikací ve třicítce jazyků a stovku titulů tuzemských i zahraničních časopisů.
</p>
<p>
Partie byla pořádána ve spolupráci se Šachovým svazem ČR.
</p>
</div>

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
      width: auto;
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
    
    <img src="/assets2/simultalka/1.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/1.jpg')" />
    <img src="/assets2/simultalka/2.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/2.jpg')" />
    <img src="/assets2/simultalka/3.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/3.jpg')" />           
    <img src="/assets2/simultalka/4.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/4.jpg')" /> 
    <img src="/assets2/simultalka/5.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/5.jpg')" />
    <img src="/assets2/simultalka/6.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/6.jpg')" />
    <img src="/assets2/simultalka/7.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/7.jpg')" />
    <img src="/assets2/simultalka/8.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/8.jpg')" />
    <img src="/assets2/simultalka/9.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/9.jpg')" />
    <img src="/assets2/simultalka/10.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/10.jpg')" />
    <img src="/assets2/simultalka/11.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/11.jpg')" />
    <img src="/assets2/simultalka/12.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/12.jpg')" />
    <img src="/assets2/simultalka/13.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/13.jpg')" />
    <img src="/assets2/simultalka/14.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/14.jpg')" />
    <img src="/assets2/simultalka/15.jpg" alt="Image 1" onclick="openModal('/assets2/simultalka/15.jpg')" />
    
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
    const imageUrls = ["/assets2/simultalka/1.jpg","/assets2/simultalka/2.jpg","/assets2/simultalka/3.jpg","/assets2/simultalka/4.jpg","/assets2/simultalka/5.jpg","/assets2/simultalka/6.jpg","/assets2/simultalka/7.jpg","/assets2/simultalka/8.jpg","/assets2/simultalka/9.jpg","/assets2/simultalka/10.jpg","/assets2/simultalka/11.jpg","/assets2/simultalka/12.jpg","/assets2/simultalka/13.jpg","/assets2/simultalka/14.jpg","/assets2/simultalka/15.jpg" ]; 
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