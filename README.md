# Analysez-les-ventes-dune-librairie-avec-R-ou-Python
# Creez-un-tableau-de-bord-dynamique-avec-Power-BI-pour-visualiser-l-avancement-de-projets
 
### Mission

Vous êtes déployé chez le client Sanitoral pour réaliser une mission de visualisation de données (appelée également dataviz).

Il s’agit d’une société internationale qui fabrique et commercialise des soins bucco-dentaires.

Sophie est cheffe de projet au sein du service Project Management Office de Sanitoral. 

Vous l’avez rencontrée pour comprendre le besoin de l’entreprise.

Son service a besoin d’un tableau de bord pour :

  - suivre l'avancement des projets et les coûts ;

  - identifier les retards ;

  - contrôler les performances, afin que l’équipe puisse mener les actions adéquates.

Vous lui envoyez la note de cadrage du projet que vous avez établie lors de votre réunion avec elle.

Avant de vous lancer dans la construction du tableau de bord, vous décidez de formaliser les user stories dans un Product Strategy Canvas à l’aide de ce modèle utilisé par les collaborateurs de ESN Data.
 
  Vous pouvez également créer un mockup de votre projet afin de vous guider dans la réalisation de votre tableau de bord (c’est le premier design de votre tableau de bord que vous allez partager avec votre mentor).

  À ce stade, faites valider votre Product Strategy Canvas par votre mentor avant de réaliser votre tableau de bord. Ne réalisez pas le tableau de bord sans avoir obtenu l'accord explicite de votre mentor !

Sophie a bien reçu votre travail et vous répond par e-mail.  
 
Bonjour,

Le Product Strategy Canvas correspond à nos besoins. Je vous donne donc mon feu vert pour réaliser le reporting ! 

Pour que nos directeurs parviennent à le lire facilement, il devra contenir des représentations graphiques lisibles et adaptées au mieux aux informations, et donner un exemple d’un axe stratégique qui peut être issu de ce reporting.

Je joins donc à cet e-mail le jeu de données que vous allez pouvoir utiliser pour réaliser le tableau de bord. 

- Les données sont extraites de notre logiciel de gestion de projets et correspondent à des projets passés entre 2018 et début 2022. 

- Vous trouverez également un dictionnaire des données pour comprendre les termes utilisés. 

Je vous laisse comprendre la structure de nos données et identifier les problèmes récurrents que nous avons eus ces dernières années.

Pour rappel, nous souhaitons mettre à jour cette analyse toutes les semaines. Nous souhaitons donc que le nettoyage des données soit automatique (il faudra utiliser Power Query Editor de l’application Power BI).

Pour finir, nous souhaitons qu’un des onglets dans Power BI soit dédié à la présentation et aux explications des éléments suivants : 

- Le Product Strategy Canvas 

- Les étapes de préparation de mise à jour des données (nous souhaitons avoir la procédure qui nous permettra de faire la mise à jour nous-mêmes) 

- Le modèle des données (explication sur les relations et les éventuelles modifications)

J’ai récemment été sensibilisée au storytelling et à son impact sur l'intérêt d’un auditoire pour une présentation, je vous mets le lien de la vidéo que j’ai vue, cela pourra certainement vous intéresser.
 
À bientôt pour la présentation du tableau de bord ! 

Sophie

### Étape 1 - Rédigez le Product Strategy Canvas

Prérequis

- Avoir lu la note de cadrage du projet.

- Avoir consulté le modèle de Product Strategy Canvas.

### Résultat attendu

- Avoir renseigné le Product Strategy Canvas qui vous permettra de comprendre les attentes des futurs utilisateurs du tableau de bord en termes de fonctionnalités.

### Recommandations

- La réalisation du PSC arrive en amont de celle du tableau de bord, pour vous permettre de gagner du temps. En effet, compléter le PSC vous permet de vous assurer d’avoir bien compris le besoin client d’abord.

- Pour clarifier les attendus, vous pouvez par exemple faire un mockup en dessinant grossièrement le rapport et les différentes visualisations que vous aurez à réaliser.

- Vous pouvez également solliciter votre mentor sur son expérience projet et la façon dont il s’organise dans les premières étapes.
 
### Étape 2 - Préparez des données dans Power Query Editor et créez un modèle de données

- Avoir installé Power BI.

- Avoir importé les données du projet dans Power BI.

- Avoir téléchargé l’extension Gantt Chart.

### Résultat attendu

- Avoir listé des étapes de préparation de données dans le Power Query Editor.

- Avoir pris une image du modèle de données que j’ai utilisé.

### Recommandations

- Les étapes de préparation de données doivent être réalisées avec PowerQuery Editor : 

  il s’agit des “étapes appliquées”, qui s’affichent à droite de l’écran lorsque vous travaillez sur le fichier de données.
<img width="558" alt="17090291207746_Capture d’écran 2024-02-27 à 05 13 18" src="https://github.com/user-attachments/assets/466a3a65-5a5f-4dd0-857c-96f7af9db421" />
 
- Il vous faudra lier les numéros des projets avec les noms des phases pour créer des clés uniques dans la table Project_Plan. Pour cela,

  vous devez utiliser la création de colonne calculée à partir des champs Project ID et Phase (exemple ci-dessous).
<img width="695" alt="17090291360318_Capture d’écran 2024-02-27 à 05 13 37" src="https://github.com/user-attachments/assets/55c193d2-ad01-43d2-80b2-e6f40a37d2d9" />

### Étape 3 - Développez le tableau de bord interactif final

### Prérequis

Avoir relu le Product Strategy Canvas pour bien avoir en tête toutes les user stories à réaliser.

### Résultat attendu

- Un tableau de bord au format .pbix.

### Recommandations 

- Il faut faire preuve d’empathie, n’oubliez pas que le tableau de bord est avant tout destiné à des directeurs. Essayez de vous demander vous même ce que vous souhaiteriez avoir comme tableau de bord si vous étiez à leurs places. 

- Mettez en évidence les retards, ou les problèmes de budget ou de livrables. Pour cela, vous pouvez avoir recours aux formules DAX. Pour vous aider à les créer, téléchargez Dax Studio. 

- Mettez en place les différents rôles dans le rapport avec les filtres sur les données.

- Gardez en tête que l’ensemble du tableau de bord sera accessible pour les 3 rôles. Comment pouvez-vous faire pour que les informations soient pertinentes pour l’ensemble des rôles sans faire une page par rôle ? 

- Essayez de trouver dans les données, des axes d’améliorations stratégiques pour faciliter la prise de décision de vos directeurs (cela peut être des indicateurs à suivre, des graphiques spécifiques, etc.)

### Points de vigilance 

- Lors de la soutenance finale, mettez-vous à la place de Sophie. Présentez-lui le tableau de bord selon ses besoins à elle (et placez-vous de son point de vue) : 

  - Suivre l’avancement des projets

  - Identifier les retards et les dérives de performance pour intervenir au plus tôt

- Soyez vigilant à la qualité de votre présentation : elle doit être synthétique, fluide, et employer un niveau de langage ni familier ni technique.

### Ressources 

- Pour vous aider dans l’utilisation de la visualisation des influenceurs clés ou Q&A, référez-vous à l’article Créer des visualisations des influenceurs clés.

- Le lien vers le site DAX Studio pour vous aider dans vos formules 

- Pour installer l’extension GANTT sur powerBI vous pouvez suivre ce tutoriel : Ajout de de GANTT sur PowerBI, Créer une info bulle dans PowerBI

### Étape 4 - Préparez la soutenance

### Résultat attendu

Le fichier Power BI au formation “.pbix” que vous présenterez à l’aide d’un support de présentation.

### Recommandations

- Lors d’une session avec votre mentor, nous vous conseillons de faire ensemble une soutenance blanche sur votre projet. Lors de cette session, vous pourrez : 

  - mettre en pratique le storytelling de votre présentation : explication des différents tableaux de bord, utilisation des rôles dans la présentation, etc ;

  - bien vérifier que vous utilisez les ingrédients et la structure du storytelling pour présenter votre travail ;

  - votre mentor pourra également vous demander de lui montrer comment il faut faire pour mettre à jour les données (chose que vous devrez faire en direct avec votre évaluateur) ;

  - votre mentor vous posera également quelques questions pour vous entraîner sur votre projet.

- Vous pouvez voir ou revoir la dernière partie du cours Développez votre culture des données pour vous inspirer des différents éléments de storytelling à mettre en place.

- Consultez la fiche d'autoévaluation pour vérifier votre travail.

 
# Analysez-des-indicateurs-de-l-egalite-femmes-hommes-en-respect-du-RGPD
 
### Mission

Vous êtes data analyst dans un cabinet de consultants spécialisé dans la transformation digitale des entreprises.

Le cabinet compte déjà plus de 150 salariés et est en plein développement.

Ce matin, en arrivant à votre poste de travail, vous recevez un email de Laura, la directrice des ressources humaines avec en copie Vincent, contrôleur de gestion sociale :

Salut, 

Comme tu le sais, chaque année avant le 1er mars, les entreprises d’au moins 50 salariés doivent calculer et publier sur leur site Internet leur index de l’égalité femmes-hommes. Nous sommes en phase de croissance importante, et il me semble important d’avoir une politique volontariste pour développer l’égalité femmes-hommes dans notre cabinet. Cela nous permettra d’améliorer notre marque employeur et d’attirer plus facilement des talents.

J’aimerais donc que tu aides Vincent à automatiser la création d’un rapport sur l’égalité professionnelle femmes hommes. Pour cela, il m’a suggéré l’utilisation de KNIME. J’aurais donc besoin qu'à partir des fichiers (en pièce jointe) issues de notre Système d’Informations des Ressources Humaines (SIRH), tu lui prépares :

- un workflow avec le logiciel KNIME qui crée les graphiques du diagnostic ;

- un fichier .csv prêt pour être utilisé dans nos futures analyses via Tableau Software.

Le site du ministère du Travail donne de nombreuses informations pour établir un diagnostic. Regarde notamment le document de présentation de lʼoutil Diagnostic Égalité dans lequel tu trouveras une liste des indicateurs à surveiller. Pas besoin de tous les extraire, mais dans un premier temps choisis-en au minimum 5 dans la liste que ton workflow devra générer.

Aussi, je te rappelle que les données issues du SIRH ne sont pas anonymisées, alors il faudra les traiter pour que ton rapport respecte le RGPD. 

Une fois que tu auras terminé, je souhaite que tu prépares un support de présentation de 15 slides maximum. 

- Tu exposeras tes résultats (données et graphiques) à tout le monde lors de la prochaine plénière de l’entreprise dans 1 mois. Cela sera l'occasion pour nous de montrer notre transparence sur ce sujet. 

- Il serait intéressant que tu y présentes ta méthodologie de collecte, d’agrégation,

  ton respect des normes réglementaires (RGPD) et ta méthode de vérification de la cohérence des données et que cette méthodologie nous permette si besoin de reproduire le processus sans erreur technique. 

- N’oublie pas de donner notre score d’égalité femmes/hommes à la fin de la présentation ainsi que des recommandations pour que notre score soit encore meilleur l’année prochaine.
 
Je reste à ta disposition en cas de besoin.

Bien à toi,

Laura Tellier

#### DRH

 
# Analysez-les-ventes-d-une-librairie-avec-R-ou-Python

### Mission

L’entreprise Lapage était originellement une librairie physique avec plusieurs points de vente. Mais devant le succès de certains de ses produits et l’engouement de ses clients, elle a décidé depuis 2 ans d’ouvrir un site de vente en ligne. 

La structure a besoin d’aide pour mieux comprendre ses données, c’est pourquoi elle vous a recruté. Vous intervenez en tant que Data Analyst afin de faire le point sur l’activité. 

L’équipe Marketing que vous intégrez se compose de : 

- Annabelle, responsable Marketing ;

- Julie, Business Intelligence Analyst.

Annabelle vous a déjà expliqué le contexte et les attendus de la mission oralement mais elle vous a fait un récapitulatif par email :
 
Hello,

Bon courage pour ta prise de poste. J’espère que tu te plairas parmi nous.

Comme tu l’as certainement compris, nous avons ouvert il y a deux ans de cela notre librairie en ligne. Sylvain, le nouveau responsable commercial, souhaite maintenant faire le point global sur les différents indicateurs et chiffres clés de l’entreprise.

Cela nous permettra de décider de la marche à suivre, par exemple décider si nous devons créer certaines offres, adapter certains prix ou cibler un certain type de clientèle etc.

Cette analyse va être découpée en deux parties :

- Une analyse des différents indicateurs de vente, qui a été demandée dans le brief (tu le trouveras en pièce jointe),

- Une analyse plus ciblée sur les clients : l’objectif est de comprendre le comportement de nos clients en ligne, pour pouvoir ensuite comparer avec la connaissance acquise via nos librairies physiques. 

Pour cela, je t’invite à voir avec Julie, qui te précisera directement ses demandes à ce niveau.

Nous avons 4 semaines pour produire cette analyse et préparer le support de présentation que tu viendras faire toi-même à Sylvain. Je te laisse libre de choisir le format de présentation que tu souhaites. 

La base de données est en pièce jointe. N’hésite pas si tu as des questions, je me tiens à ta disposition.
 
Excellente journée à toi !

#### Annabelle

#### PS1 : N’oublie pas que Sylvain et ses équipes n’ont pas de connaissances techniques, il faut essayer d’être le plus clair possible. 

#### PS2 : Tu vas faire ta présentation pendant le CODIR de Sylvain et nous n’avons que 15 minutes. Donc nous attendons de toi une posture adaptée de conseil stratégique pour la direction.
 
### Quelques instants plus tard

Après avoir consulté le mail d'Annabelle, vous prenez directement contact avec Julie sur Teams.

![16992603146474_image7](https://github.com/user-attachments/assets/0f0e46bf-7217-4713-bfc3-95ccf3f493cf)

