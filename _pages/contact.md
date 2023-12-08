---
layout: single
title: Contactez-nous
permalink: /contact/
---


Nous sommes ici pour répondre à toutes vos questions concernant la location de livres d'or audio.

## Nous Joindre

- **Email :** lefilasouvenirs@gmail.com
- **Téléphone :** +33 6 45 17 56 69
- **Adresse :** Toulouse et ses environs

## Demandez un devis !

<form action="https://formspree.io/f/mjvqnkjj" method="POST">
  <label>
    Nom :
    <input type="text" name="nom">
  </label>
  <label>
    Prénom :
    <input type="text" name="prenom">
  </label>
  <label>
    Téléphone :
    <input type="tel" name="telephone">
  </label>
  <label>
    E-mail :
    <input type="email" name="email">
  </label>
    <label>
    Durée de l'événement :
    <select name="duree_evenement" id="duree_evenement">
      <option value="0">Soirée</option>
      <option value="100">Week-End</option>
    </select>
  </label>
      <label>
    Choix de la formule :
    <select name="formule" id="formule">
      <option value="150">Décoration incluse</option>
      <option value="100">Téléphone seul</option>
    </select>
  </label>

  <fieldset>
    <legend>Options supplémentaires :</legend>
    <label>
      <input type="checkbox" name="option_pdf" id="option_pdf"  value="30"> Rendu pdf avec audio transcrit
    </label>
    <!-- Ajoutez d'autres cases à cocher ici selon vos besoins -->
  </fieldset>

  <label>
    Choisissez votre événement :
    <select name="type_evenement">
      <option value="">--Choisissez une option--</option>
      <option value="">Mariage</option>
      <option value="">Anniversaire</option>
      <option value="">Crémaillère</option>
    </select>
  </label>
  <label>
    Adresse du lieu de l'événement (En cas d'installation & retrait du matériel) :
    <input type="text" name="adresse_evenement">
  </label>
  <!-- Ajoutez d'autres champs similaires pour les autres sélections -->
  <label>
    Date de l'événement :
    <input type="date" name="date_evenement">
  </label>
  <label>
    Choix de livraison :
    <select name="choix_livraison" id="choix_livraison">
      <option value="0">Click and Collect (à récupérer sur Toulouse)</option>
      <option value="50">Livraison sur le lieu de l'événement</option>
    </select>
  </label>
  <label>
    Comment avez-vous découvert Le fil à souvenirs ?
    <textarea name="decouverte_filasouvenirs"></textarea>
  </label>

  <label>
    Une Question ? Une remarque ?
    <textarea name="question"></textarea>
  </label>

    <p>Prix estimé : <span id="prix">0</span> €</p>

  <button type="submit">Envoyer</button>
</form>


Vous pouvez également nous laisser un message en utilisant notre page [instagram](https://www.instagram.com/lefilasouvenirs/).

<script>
  // Fonction pour calculer le prix
  function calculerPrix() {
    var prix = 0;
    
    // Ajoutez votre logique de calcul ici
    // Par exemple, ajouter un certain montant si une case spécifique est cochée
    // Calcul pour l'option PDF
    if (document.getElementById('option_pdf').checked) {
      prix += parseInt(document.getElementById('option_pdf').value);
    }

    // Calculer le supplément en fonction du choix de livraison
    var choixLivraison = document.getElementById('choix_livraison').value;
    prix += parseInt(choixLivraison);

    // Calculer le supplément en fonction du choix de livraison
    var formule = document.getElementById('formule').value;
    prix += parseInt(formule);

    // Calculer le supplément en fonction du choix de livraison
    var duree_evenement = document.getElementById('duree_evenement').value;
    prix += parseInt(duree_evenement);

    // Afficher le prix calculé
    document.getElementById('prix').textContent = prix;
  }

  // Attacher l'écouteur d'événements à tous les éléments pertinents
  document.querySelectorAll('input[type=checkbox], select').forEach(function(element) {
    element.addEventListener('change', calculerPrix);
  });

  // Initialiser le prix au chargement de la page
  window.onload = calculerPrix;
</script>


<style>
@import url('https://fonts.googleapis.com/css?family=Spartan&display=swap');

/* Couleurs et styles de base */
:root {
  --form-bg: #f8f4e5;
  --form-border: #f45702;
  --form-focus: #6bd4b1;
  --font-size: 16px;
  --font-face: 'Spartan', sans-serif;
  --font-color: #2A293E;
}




body {

    background-size: cover;
  background-attachment: fixed;
  display: flex;
  align-items: center;

  height: 100vh;
  font-family: var(--font-face);
  color: var(--font-color);
}

form {
  background: var(--form-bg);
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  width: 100%;
  max-width: 500px;
}

label {
  margin-bottom: 10px;
  display: block;
  font-size: var(--font-size);
}

input[type="text"],
input[type="email"],
input[type="tel"],
input[type="date"],
select,
textarea {
  width: 100%;
  padding: 8px;
  margin-bottom: 20px;
  border-radius: 4px;
  border: 1px solid #ccc;
  font-family: var(--font-face);
  font-size: var(--font-size);
}

input[type="checkbox"] {
  margin-right: 10px;
}

button {
  background: var(--form-border);
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-size: var(--font-size);
  font-family: var(--font-face);
  transition: background 0.3s ease;
}

button:hover {
  background: var(--form-focus);
}

/* Style pour le prix estimé */
#prix {
  font-weight: bold;
  color: var(--form-border);
}

fieldset {
  border: none;
  margin-bottom: 20px;
}

legend {
  font-weight: bold;
  margin-bottom: 10px;
}

#site-nav.greedy-nav {
  background-color: transparent;
}

/* Si vous souhaitez également rendre les liens visibles sur un fond transparent */
#site-nav.greedy-nav a {
  color: black; /* ou toute autre couleur qui ressort bien sur votre fond */
}

/* Style pour les éléments de la liste */
#site-nav.greedy-nav ul.visible-links li.masthead__menu-item {
  list-style-type: none; /* Pour enlever les puces */
}

/* Style pour le bouton de menu en mode responsive */
button.greedy-nav__toggle {
  background-color: black; /* Vous pouvez changer cette couleur */
  color: #ffffff; /* Couleur du texte */
  border: none;
  padding: 10px;
}

button.greedy-nav__toggle .navicon {
  /* Ajoutez ici le style pour la représentation visuelle du bouton (icon) */
}

/* Style pour les liens cachés */
ul.hidden-links.hidden li.masthead__menu-item {
  list-style-type: none; /* Pour enlever les puces */
}


</style>