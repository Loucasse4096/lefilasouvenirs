---
layout: post
title:  "Anniversaire Maxime !"
date:   2023-03-15 16:16:01 -0600
categories: mariage
gallery:
  - url: https://drive.google.com/uc?export=view&id=1p0rPROTg8OglAxeu4l76yCStbelFbana
    image_path: https://drive.google.com/uc?export=view&id=1p0rPROTg8OglAxeu4l76yCStbelFbana
    alt: "placeholder image 1"
    title: "Anniversaire de Maxime !"
  - url: https://drive.google.com/uc?export=view&id=1vNvfFKqOMPl8bGneCyC3NXn3UHsZa4DD
    image_path: https://drive.google.com/uc?export=view&id=1vNvfFKqOMPl8bGneCyC3NXn3UHsZa4DD
    alt: "placeholder image 2"
    title: "Anniversaire de Maxime !"
  - url: https://drive.google.com/uc?export=view&id=1WC6XdUcaaiGuzhp1OpuTilnfFHMzOiEW
    image_path: https://drive.google.com/uc?export=view&id=1WC6XdUcaaiGuzhp1OpuTilnfFHMzOiEW
    alt: "placeholder image 1"
    title: "Anniversaire de Maxime !"
  - url: https://drive.google.com/uc?export=view&id=1uY6pc-1B7LxcuvGFu-jYbfcQw6ITWWzn
    image_path: https://drive.google.com/uc?export=view&id=1uY6pc-1B7LxcuvGFu-jYbfcQw6ITWWzn
    alt: "placeholder image 2"
    title: "Anniversaire de Maxime !"

---

Anniversaire de Maxime !

<a href="javascript:history.back()" class="back-button">
  &#8592; Retour
</a>

<ul>
  {% for item in page.gallery %}
    <li>
      <a href="{{ item.url | relative_url }}" onclick="openModal(this); return false;">
        <figure>
          <img src="{{ item.url | relative_url }}" alt="{{ item.title }}">
          <figcaption>{{ item.title }}</figcaption>
        </figure>
      </a>
    </li>
  {% endfor %}
</ul>

<div id="lightbox-modal" onclick="closeModal()">
  <span class="close">&times;</span>
  <img id="lightbox-image" src="" alt="">
  <p id="lightbox-caption"></p>
</div>


<style>

#lightbox-modal {
  display: none;
  position: fixed;
  z-index: 1000;
  padding-top: 100px;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: auto;
  background-color: rgb(0,0,0);
  background-color: rgba(0,0,0,0.9);
}

#lightbox-modal img {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
}

.close {
  position: absolute;
  top: 15px;
  right: 35px;
  color: #fff;
  font-size: 40px;
  font-weight: bold;
  cursor: pointer;
}


.back-button {
  position: fixed;
  top: 10px;
  left: 10px;
  background-color: #f4f4f4;
  color: #333;
  padding: 10px;
  border-radius: 5px;
  text-decoration: none;
}

* {
	box-sizing: border-box;
}

body {
	font-family: Lato, sans-serif;
	margin: 0;
	padding: 1rem;
	min-height: 100vh;
	display: flex;
	justify-content: center;
	align-items: center;
	background: rgba(20, 20, 20, 1);
}

img {
	width: 100%;
	display: block;
	aspect-ratio: 1 / 1;
	object-fit: cover;
	transition: transform 1000ms;
}

ul {
	list-style: none;
	margin: 0;
	padding: 0;
	display: grid;
	gap: 0.5rem;
	grid-template-columns: repeat(auto-fit, minmax(20rem, 1fr));
	max-width: 100%;
	width: 70rem;
}

figure {
	margin: 0;
	position: relative;
	overflow: hidden;
}

figure::after {
	content: '';
	position: absolute;
	top: 50%;
	left: 50%;
	width: 200%;
	height: 200%;
	background: rgba(0, 0, 0, 0.5);
	transform-origin: center;
	opacity: 0;
	transform: scale(2);
	transition: opacity 300ms;
}

figcaption {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	display: flex;
	justify-content: center;
	place-items: center;
	text-align: center;
	padding: 1rem;
	color: white;
	font-size: 1.2rem;
	z-index: 1;
	opacity: 0;
	transition: opacity 600ms, transform 600ms;
}

a:is(:hover, :focus) figure::after {
	opacity: 1;
}

a:is(:hover, :focus) figcaption {
	opacity: 1;
	transition: opacity 600ms;
}

@media (prefers-reduced-motion: no-preference) {
	figcaption {
		transform: translate3d(0, 2rem, 0);
	}
	
	figure::after {
		border-radius: 50%;
		opacity: 1;
		transform: scale(0);
		transition: transform 900ms;
	}
	
	a:is(:hover, :focus) figure::after {
		transform: scale(2.5);
	}

	a:is(:hover, :focus) figcaption {
		opacity: 1;
		transform: translate3d(0, 0, 0);
		transition: opacity 600ms 400ms, transform 600ms 400ms;
	}

	a:is(:hover, :focus) img {
		transform: scale(1.2);
	}
}


</style>

<script>
function openModal(anchor) {
  var modal = document.getElementById("lightbox-modal");
  var modalImg = document.getElementById("lightbox-image");
  var captionText = document.getElementById("lightbox-caption");
  modal.style.display = "block";
  modalImg.src = anchor.href;
  captionText.innerHTML = anchor.children[0].children[1].innerHTML;
}

function closeModal() {
  var modal = document.getElementById("lightbox-modal");
  modal.style.display = "none";
}

</script>