1. L'exemple du "modèle événement → état → rendu" est tel que peut décrire le déroulement d'un code comme l'exemple de l'extrait 5 de la Partie 4, ci-dessous;

const items = document.querySelectorAll('.faq-question');

items.forEach((item) => {
  item.addEventListener('click', () => {
    item.nextElementSibling.classList.toggle('is-visible');
  });
});

>> La ligne 3 est l'information que l'on va lié à l'action (ligne 5), l'évènement avec '.addEventListener' (ligne 6) va s'activer si il y'a une intéraction par l'utilisateur avec un simple clique, l'état sera l'élément, la réponse est ou non visible 'is-visible' et le rendu, son résultat affichera ou masquera la réponse de la FAQ.

2.  classList.toggle est la passerelle entre JS et CSS, concernant tout ce qui est intéraction, le JS peut procéder à cela contrairement au CSS qui ne peut pas le faire, pour rappel, le CSS n'a pour but que l'apparence d'un site.

Je n'ai pas procédé à l'utilisation d'une Intelligence Artificielle, je me suis simplement aidé et repris des définitions du cours dans les précédents TP/TD sur Moodle
