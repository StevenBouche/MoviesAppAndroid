# The Moovie App

## Organisation

- Steven Bouche

## Objectifs
Dans ce projet, nous allons créer l'application AnneFlix (The new Netflix). L'objectif est d'exploiter la base de données TheMoovieDB (https://developers.themoviedb.org/3) afin de permettre aux utilisateurs de l'application de visualiser, noter et voir la bande annonce des films de la base de données. 

## Fonctionnalités 

- Deux langues prise en compte EN / FR (traduction)

- Fragment Authentification : 
  - Géneration du RequestToken
  - Authentification au compte utilisateur en validant le token au compte
  - Génération de la session utilisateur 

![login](/img/login.png)

- Fragment Home :
  - Visualisation du film vedette du moment
  - Visualisation de plusieurs rubrique de films, en tendance, au cinéma, qui arrive bientôt, ainsi que les tops film 
  - Redirection vers un fragment permettant de voir tous les films des différentes rubriques 
  - Redirection vers un fragment affichant les détails d'un film lorsque l'on clique sur sa vignette 

![home](/img/home.png)

- Fragment Recherche :
  - Affiche tous les films en rapport avec un mot saisi dans la barre de recherche
  - Scroll infini avec la pagination 
  - Redirection vers un fragment affichant les détails d'un film lorsque l'on clique sur sa vignette

![search](/img/search.png)

- Fragment Genres :
  - Liste tous les genres possibles de l'API
  - Redirection vers un fragment pour visualiser tous les films d'un certain genre avec possibilité de trie

![genre](/img/genre.png) ![genre2](/img/genre2.png)

- Fragment Détails d'un film :
  - Affiche sa photo de couverture, son titre, ses genres, ses votes, sa note moyenne, sa date de sortie, sa durée, sa langue et sa description
  - Possibilité de le mettre dans ma liste de favoris 
  - Possibilité de lui donner une note 
  - Affiche tous ses trailers et si l'on clique dessus redirige un fragment pour lancer la vidéo
  - Affiche le casting du film
  - Affiche les films similaires
  - Redirection vers un fragment affichant les détails d'un film lorsque l'on clique sur sa vignette dans les films similaires
  - Redirection vers fragment youtube et de consultation des critiques du film

![details](/img/details.png) ![details2](/img/details2.png)

- Fragment Favoris :
  - Permets la consultation de tous les films que l'on a mis en favoris
  - Redirection vers un fragment affichant les détails d'un film lorsque l'on clique sur sa vignette
    
![favorite](/img/favorite.png)

## Navigation

![navigation](/img/navigation.png)

## Librairies
- Navigation-fragment 
- Hilt : Injection de dépendances 
- Gson/Moshi : Sérialisation et Désérialisation JSON 
- Retrofit: Pour consommer l'API The Moovie DB
- Picasso/Glide/Coil/ : Pour afficher les images 
- OkHttp: Client HTTP
- androidyoutubeplayer
- RxAndroid / RxJava



