---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: single
excerpt: "Bienvenue dans une nouvelle ère des souvenirs. Le livre d'or audio réinvente la tradition en capturant les voix et les émotions de vos invités."
header:

  carousel: true

  actions:
    - label: "Découvrez nos offres"
      url: "/nosformules"
---







<figure class="half">
    <figcaption>Nos Coloris</figcaption>
    <img src="assets/images/index/4.png">
    <img src="assets/images/index/5.png">
</figure>

<figure class="third">
	<img src="assets/images/index/1.png">
	<img src="assets/images/index/2.png">
	<img src="assets/images/index/3.png">
</figure>



<div class="advantages-section">
    <div class="advantages-content">
        <h2>Pourquoi Choisir un Livre d'Or Audio ?</h2>
        <ul>
            <li>Authenticité : Capturez l'émotion réelle et les intonations des messages.</li>
            <li>Facilité d'Utilisation : Accessible à tous, enregistrez un message en quelques clics.</li>
            <li>Souvenirs Durables : Réécoutez ces messages quand vous le souhaitez.</li>
        </ul>
    </div>
    <div class="advantages-image">
          <img src="/assets/images/index/index_1.jpg" alt="Description de l'image">
    </div>
</div>


<div class="how-it-works-section">
  <h2>Comment ça Marche ?</h2>
  <ol>
    <li>Enregistrement : Les invités utilisent leur téléphone pour enregistrer leur message.</li>
    <li>Collecte : Nous collectons tous les enregistrements.</li>
    <li>Présentation : Les messages sont compilés dans votre livre d'or audio personnalisé.</li>
  </ol>
</div>

<div class="how-it-works-section">
  <h2>Notre engagement</h2>
    <p>Nous proposons nos services à Toulouse et dans un rayon de 20 min, limitant ainsi les déplacements. Nous proposons également un service Clik and Collect permettant à nos clients ou leur entourage de venir récupérer notre matériel.</p>
</div>



<div class="faq-section">
  <h2>FAQ</h2>
  <p><strong>Q</strong> : Combien de temps les messages peuvent-ils durer ?</p>
  <p><strong>R</strong> : Chaque message peut durer jusqu'à 2 minutes.</p>
</div>

<div class="call-to-action-section">
  <h2>Prêt à Créer Votre Livre d'Or Audio ?</h2>
  <p><a href="/contact">Contactez-nous</a> pour plus d'informations ou pour commencer.</p>
</div>



<style>

/* Style global pour les figures */
figure {
    margin: 20px auto; /* Centrage et espacement autour de chaque groupe d'images */
    text-align: center; /* Alignement central pour les éléments à l'intérieur */
}

/* Style pour les images */
figure img {
    width: 100%; /* Largeur complète pour s'adapter au conteneur parent */
    height: auto; /* Hauteur automatique pour maintenir le ratio de l'image */
    border-radius: 5px; /* Bords arrondis pour un look doux */
    box-shadow: 0 4px 8px rgba(0,0,0,0.2); /* Ombre légère pour un effet de profondeur */
    margin: 10px; /* Espacement entre les images */
}

/* Style pour les figures avec classe 'third' */
.third img {
    max-width: 30%; /* Maximum 30% de la largeur pour chaque image */
}

/* Style pour les figures avec classe 'half' */
.half img {
    max-width: 45%; /* Maximum 45% de la largeur pour chaque image */
}

/* Style spécifique pour la légende 'Nos Coloris' */
.half figcaption {
    text-align: center; /* Centrage du texte */
    color: #444; /* Couleur du texte */
    font-family: 'Arial', sans-serif; /* Police de caractères */
    font-size: 24px; /* Taille de la police plus grande */
    font-weight: bold; /* Police en gras */
    margin-bottom: 20px; /* Espacement sous le titre */
}

/* Style de base pour les sections */
.advantages-section, .how-it-works-section, .faq-section, .call-to-action-section {
    background-color: #f9f9f9; /* Fond blanc pour plus de clarté */
    color: #353b48;
    font-family: 'Arial', sans-serif; /* Police cohérente avec le reste du design */
    padding: 25px; /* Padding augmenté */
    margin: 25px 0;
    border-radius: 12px; /* Bords plus arrondis */
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    font-family: serif;
}

/* Titres des sections */
.advantages-section h2, .how-it-works-section h2, .faq-section h2, .call-to-action-section h2 {
    color: #273c75; /* Couleur de titre modifiée pour plus d'élégance */
    font-size: 30px; /* Taille de la police augmentée pour les titres des sections */
    text-transform: uppercase; /* Mise en majuscule des titres */
    font-weight: bold; /* Police en gras */
    margin-bottom: 20px;
    text-align: center; /* Centrage des titres */
    font-family: "Gill Sans", sans-serif;
}

/* Listes */
.advantages-section ul, .how-it-works-section ol {
    padding-left: 30px; /* Padding de la liste ajusté */
}

/* Questions et Réponses de la FAQ */
.faq-section p {
    margin-bottom: 15px;
}

/* Bouton d'appel à l'action */
.call-to-action-section p {
    text-align: center;
}

.call-to-action-section a {
    background-color: #007bff;
    color: white;
    padding: 12px 24px; /* Padding légèrement plus grand */
    border-radius: 6px;
    text-decoration: none;
    display: inline-block;
    margin-top: 15px;
    transition: background-color 0.3s ease-in-out; /* Transition pour le bouton */
}

.call-to-action-section a:hover {
    background-color: #0056b3;
    box-shadow: 0 4px 8px rgba(0,0,0,0.15); /* Ombre légère au survol */
}

/* Style pour les images dans les sections */
.section-image {
    width: 100%;
    height: auto;
    margin-bottom: 25px;
    border-radius: 12px;
}

/* Responsive design pour les petits écrans */
@media (max-width: 800px) {
    .advantages-section, .how-it-works-section, .faq-section, .call-to-action-section {
        padding: 20px;
    }

    .advantages-section {
        flex-direction: column;
    }

    .advantages-image img {
        width: 90%; /* Largeur ajustée pour petits écrans */
        margin: 20px auto;
    }
}

/* Flexbox pour les sections avantages */
.advantages-section {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: #f9f9f9;
    padding: 20px;
    margin: 20px 0;
    border-radius: 10px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.advantages-content, .advantages-image {
    flex: 1;
}

.advantages-image img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    margin-left: 20px;
}

/* Ajouts pour correspondre à l'image fournie */
/* Titre principal */
.main-title {
    font-size: 48px; /* Taille de la police plus grande pour le titre principal */
    color: #002366; /* Couleur du titre principal */
    text-align: center; /* Centrage du titre */
    margin-bottom: 30px; /* Espacement après le titre */
    font-weight: normal; /* Pas de gras pour le titre principal */
}

/* Sous-titre pour engagement */
.subtitle-engagement {
    font-size: 22px; /* Taille de la police pour les sous-titres */
    color: #002366; /* Couleur pour les sous-titres */
    text-align: center; /* Centrage du sous-titre */
    font-weight: bold; /* Police en gras pour les sous-titres */
    margin: 20px 0; /* Espacement autour du sous-titre */
    text-transform: uppercase; /* Mise en majuscule du sous-titre */
}

/* Paragraphe de l'engagement */
.engagement-text {
    font-size: 18px; /* Taille de la police pour le paragraphe */
    color: #002366; /* Couleur pour le paragraphe */
    text-align: center; /* Centrage du paragraphe */
    margin: 20px 0 30px; /* Espacement autour du paragraphe */
    font-weight: 300; /* Police plus fine pour le paragraphe */
}






</style>








