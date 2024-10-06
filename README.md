## Adresse de la page 
https://luceg02.github.io/devmaisoncssgiovannetti/

### Header
#### HTML
Le <header> est structuré en deux parties : un logo et une barre de recherche. Le logo est placé à l'aide de Bootstrap dans un <div> de classe <col-5 myLogo>, contenant une image. La barre de recherche se localise dans une <div> de classe <col-3>.

#### CSS
Le header utilise Flexbox (<display: flex>), avec <justify-content: space-between> pour créer un espacement optimal. Les éléments sont centrés verticalement grâce à <align-items: center>.
Le formulaire de recherche utilise également Flexbox.

### Navbar
#### CSS
Le menu utilise Flexbox (display: flex), ce qui permet aux éléments d'avoir une largeur égale (flex: 1), tout en éliminant les marges et le padding par défaut.
Les liens de menu (a) sont stylisés sans soulignement et avec des espaces internes. Ils sont dotés d'une couleur de fond <aliceblue> et d'une bordure.
Lors du survol, la couleur de fond change. Les sous-menus sont masqués par défaut et s'affichent lorsqu'un utilisateur survole leur parent.

### Fil d'Ariane
#### HTML
Le fil d'Ariane est structuré au sein d'une <div> avec la classe <row>.

#### CSS
La classe <.breadcrumbs> élimine les puces par défaut (list-style-type: none).
La police est définie à une taille de 14 pixels, avec une couleur bleue.
Chaque élément de la liste est affiché en ligne grâce à <display: inline>.
Les liens (.breadcrumbs li a) sont stylisés sans soulignement.

### Main
#### HTML
Le conteneur principal est une <section class="row"> qui utilise Bootstrap pour diviser l'espace en colonnes. 
Le main occupe 9 colonnes.
Trois cards sont ensuite présentées dans des <div class="col-4 carte">.
#### CSS
L’en-tête (#entete) a une couleur bleue et le texte est blanc pour le titre (#contenu h1).
Les cartes sont stylisées avec un fond clair (aliceblue) et des ombres.
Les bords des cartes sont arrondis et le premier et le dernier enfant de <.carte> bénéficient d'un style spécifique pour les coins.
Les listes à l'intérieur des cartes n'ont pas de puces, et chaque élément de liste est espacé.

### Aside
#### HTML
La section <aside> occupe trois colonnes, et est divisée en deux parties :
La première partie est un <div class="myaside aside1">.
La seconde partie est un <div class="myaside aside2">.
#### CSS
Les titres de section ont un style gras et en majuscules.
Les liens dans les listes n'ont pas de soulignement par défaut, mais ils deviennent soulignés au survol.
Les marges et le padding ont été ajustés.

### Footer
#### HTML
Le footer contient un <div class="row">.
#### CSS
Le fond de <#bas_page> est d'un bleu vif (#199bdb), les éléments de la liste sont disposés en utilisant Flexbox (display: flex;), permettant une répartition des catégories avec un espacement entre elles (gap: 1.5em).
Les sous-listes ont des puces de type <disc>.
Le <#fin_footer> a un fond plus sombre (#042353), et il est centré avec un texte en petite taille.

### Media Query pour responsive appareils mobiles
Cette media query cible les écrans ayant une largeur maximale de 767,98 pixels, ce qui est typique pour les smartphones. Tous les <div> enfants directs de <.row> à l'intérieur de la balise <main> sont configurés pour occuper 100 % de la largeur de leur conteneur. Cela permet d’assurer que les éléments s'affichent en pleine largeur sur les petits écrans. De plus, un espacement de 15 pixels est ajouté en bas de chaque élément pour créer une séparation visuelle.

### Media Query pour menu responsive appareils mobiles
Cette deuxième media query, cible les mêmes conditions que la première, est utilisée pour modifier l'affichage du menu de navigation sur les écrans mobiles. Le menu devient vertical (display: block). Chaque élément du menu (<li>) est également configuré pour occuper 100 % de la largeur.
