# Analyse-Ventes-projet-EXCEL
<br>
<b><h1> 📊Analyse des données de ventes – Projet Data Analyst( Excel & Power Query)<h2></h2></b><br>
<br>
<b><h3>Présentation du projet</h3></b><br>
  <br>
Ce projet présente une analyse complète d’un jeu de données de ventes afin d’identifier des informations utiles pour la prise de décision.<br>
  <br>
<b><h3>Problématique</h3></b><br>
  <br>
Les entreprises disposent souvent de grandes quantités de données de vente, mais il est parfois difficile d’en extraire des informations pertinentes.<br>
<br>
L’objectif de ce projet est d’analyser les données afin de répondre à plusieurs questions stratégiques liées à la performance commerciale.<br>
<br>
<b><h3>Objectifs de l’analyse</h2></b>
  <br>
Les principaux objectifs de cette analyse sont :<br>
<br>
* analyser la performance globale des ventes<br>
* identifier les produits les plus performants<br>
* analyser la performance des ventes par région<br>
* étudier la performance des commerciaux<br>
* identifier les segments clients les plus rentables<br>
  <br>
<b><h3>Description du dataset</h3></b><br>
<br>
Le jeu de données contient <b>1000 transactions</b> de vente avec les variables suivantes :<br>
<br>
* Sale_ID<br>
* Date<br>
* Region<br>
* City<br>
* Salesperson<br>
* Product<br>
* Category<br>
* Quantity<br>
* Unit_Price<br>
* Channel<br>
* Customer_Segment<br>
<br>
<b><h3>Outils utilisés</h3></b><br>
<br>
* Microsoft Excel<br><br>
* Power Query<br>
* Tableaux croisés dynamiques<br>
* Visualisation de données<br>
  <br>
<p align="center">
  <img src="Images\Données_Brutes.png" alt="Vu Exel" width="600">
    <br>
      <b>Image de données Brut via Excel</b>
</p>
<br>
<b><h2>Etape 1: Nettoyage et préparation des données(Power Query></h2></b><br>
<br>
Avant toute analyse; j'ai procédé à un audit complet du dataset via<b> Power Query></b> pour garantir l'intégrité des resultats. Le processus de <b>Nettoyage et Transfromation</b> s'est articulé autour de deux axes:<br>
<br>
<b>1. Examen de la structure et Qualité</b><br>
  **<b>Vérification de la coherence:</b> Audit des colonnes pour répérer les erreurs de saisie.<br>
  **<b>Normalisation:</b> Harmonisation des casses pour éviter les doublons lors des regroupements.<br>
  <br>
<b>2. Typage et Préparation</b><br>
**<b>Données monétaires:</b> Conversion des prix et montants en format <b>Nombre décimal</b><br>
**<b>Données Temporelles:</b> Définition stricte du format <b>Date</b> pour activer les hiérarchies chronologiques.<br>
<br>
<b>3. Enrichissement du Modèle</b><br>
Afin d'affiner l'analyse, j'ai créé des colonnes calculées directement dans <b>Power Query:</b>
  **<b>Calendrier:</b> Extraction automatique de l'<b>année</b>,du <b>Mois</b>, et du <b>N° de Mois</b> pour une analyse précise de saisonnalité.<br>
  **<b>Calcul métier:</b> Création de la colonne <b>Chiffre d'affaire</b> (Quantité x Prix Unitaire).<br>
  <br>
  <table align="center">
      <tr>
        <td align="center">
          <img src="Images\P_Qwery_Type_de_données.png" width="400">
          <br>
          <b>Transformation de données</b>
        </td>
      <td align="center">
           <img src="Images\New_Table_after_PowerQuery.png" alt="after Power Query" width="400">
            <br>
            <b>After Power Query</b>
      </td>
      </tr>
  </table>
  <br>
<b><h2>🔄 Étape 2 : Transformation et Modélisation</h2></b><br>
<br>
Une fois les données assainies, j'ai structuré la phase de transformation pour répondre aux besoins analytiques de la direction. Cette étape a permis de passer d'une base de données brute à un <b>modèle prèt pour l'analyse décisionnelle<br>
<br>
<b><h2>1. Analyse Temporelle</h2></b><br>
  *<b>Objectif:</b> Etudier l'évolution de l'activité sur les exercices 2024 et 2025.<br>
  *<b>Action:</b> Regroupement chronologique par trimestres et mois pour identifier les cycles de vente et les périodes de forte croissance. trouverz sur les images les analyses matricielle pour motrer l'évolution du <b>Chiffre d'affaire</b> dans le temps  et l'analyse chronologique pour détecter les pics en fonction des mois<br>
  <br>
<table align="center">
  <tr>
    <td align="center">
      <img src="Images\1_Analyse_Temprelle.png" width="700">
      <br>
        <b>Graphique et TCD Matricielle de l'AT</b>
    </td>
    <td align="center">
      <img src="Images\2_Analyse_temporelle.png" width="600">
      <br>
        <b>Grphique et TCD Chronologique de l'AT</b>
    </td>
  </tr>
</table>
<br>
<b><h2>2. Analyse Commerciale</h2></b><br>
Cette section vise à analyser la performance des vendeurs à travers le chiffre d’affaires qu’ils génèrent.
L’objectif est d’identifier les vendeurs les plus performants et de comparer leur contribution aux ventes totales de l’entreprise.<br>
<br>
Pour cela, le chiffre d’affaires a été analysé et comparé entre les différents vendeurs afin de mieux comprendre leur impact sur la performance commerciale globale.<br>
<p align="center">
  <img src="Images\Analyse_Commerciale.png" width="600">
  <br>
  <b>Graphique et TCD du CE par vendeur</b>
</p>
<br>
<b><h3>Analyse Géographique</h3></b><br>
Cette section vise à analyser la performance des vendeurs à travers le chiffre d’affaires qu’ils génèrent.
L’objectif est d’identifier les vendeurs les plus performants et de comparer leur contribution aux ventes totales de l’entreprise.<br>
<br>
Pour cela, le chiffre d’affaires a été analysé et comparé entre les différents vendeurs afin de mieux comprendre leur impact sur la performance commerciale globale.<br>
<p align="center">
  <img src="Images\Graph_Vente_Region.png" width="600">
  <br>
  <b>Graphique et TCD du CA en fonction des Regions</b>
</p>
<br>
<b><h4>Analyse par PRODUIT</h4></b><br>
Cette section vise à analyser la performance des différents produits en fonction du chiffre d’affaires généré.
L’objectif est d’identifier les produits les plus performants ainsi que ceux qui contribuent le plus aux ventes de l’entreprise.<br>
<br>
Cette analyse permet de mieux comprendre la contribution de chaque produit à la performance commerciale globale et d’identifier les produits à fort potentiel.<br>
<p align="center">
  <img src="Images\Grap_Vente_Produit.png" width="600">
  <br>
  <b>Graphique et TCD du CA par PRODUIT</b>
  <br>
</p>
<br>
<b><h2> Analyse EPLORATIVE</h2></b><br>
<br>
Cette section présente une analyse exploratoire des données de vente afin de mieux comprendre la structure du dataset et d’identifier les principaux facteurs influençant la performance commerciale.<br>
<br>
L’objectif est d’examiner plusieurs dimensions des ventes, notamment la performance globale, la contribution des produits, la rentabilité des villes, la performance des commerciaux, l’importance des segments clients ainsi que l’efficacité des différents canaux de vente.<br>
<br>
Cette analyse permet de dégager une première compréhension des tendances présentes dans les données et de mettre en évidence les principaux leviers de performance commerciale.<br>
<br>
<b><h3>1. Performance Global des Ventes</h3></b><br>
  <br>
Cette analyse présente la contribution mensuelle au chiffre d’affaires annuel pour les années 2024 et 2025.
L’objectif est de comprendre la répartition des ventes au cours de l’année et d’identifier les périodes qui génèrent la plus grande part du chiffre d’affaires.<br>
<br>
Le tableau croisé dynamique et le graphique permettent de visualiser la part du chiffre d’affaires mensuel par rapport au chiffre d’affaires annuel, afin de mettre en évidence les variations et les tendances entre les deux années.<br>
<p align="center">
 <img src="Images\CA_GLOBAL_par_AN.png" width="600">
   <br>
   <b>Graphique des performances annuelle</b>
</p>
<br>
<b><h3>2. Les Produits les plus performants </h3></b><br>
<br>
comprendre quels produits dominent le marché est crutial pour toute prise de décision basée sur l'analyse de données. A travers cette implémentation , je cherche à transformer des données brutes en connaissance actionnables pour prioriser les investissements et maximiser la rentabilité globale.<br>
<p align="center">
  <img src="Images\Perf_Produit.png" width="600">
  <br>
    <b>Performance des Produits</b>
</p>
  <br>
  <b><h3>3. Les Villes les plus performances</h></b><br>
  Cette étape de l'analyse vise à isoler les zones géographiques les plus rentables .En corrélant le volume du CA ( chiffre d'affaire) par Ville. L'objectif est de cartographier les centres de profits majeurs.<br>
  Cette analyse est crutiale pour prioriser les zones de stockage ou les circuits de livraisons.<br>
  <p align="center">
    <img src="Images\Perf_Regions.png" width="600">
      <br>
      <b>Performantion Géographique</b>
  </p>
  <br>
  <b><h3>4. Performance des Commerciaux</h3></b><br>
  Cette analyse vise à comprendre comprendre la dynamique humaine dèrrière les chiffres. En segmentant par agent, nous cherchons à identifier les modèles de réussites.<br>
  <p align="center">
    <img src="Images\Perf_Vendeurs.png" width="600">
    <br>
    <b>Performance en fonction des vendeurs</b>
  </p>
    <br>
    <b><h3>5. Les segments client les plus performants</h3></b><br>
Cette section vise à catégoriser la base client pour identifier les groupes les plus rentables.En analysant la performance par segment, l'objectif est de comprendre quels profils tirent la croissance de l'activité .
<p align="center">
  <img src="Images\Perf_Segment.png" width="600">
  <br>
  <b>Performance par Segment Client</b>
</p>
<br>
<b><h3>6. Les Canaux de vente les plus Performants</h3></b><br>
Cette section évalue l'éfficacité de nos differents points de contact avec le client. En comparant le <b>chiffre d'affaire</b> et <b>le volume de transaction</b> par canal; l'objectif est d'identifier les vecteurs de vente les plus rentables.
  <p align="center">
    <img src="Images\Perf_Canal.png" width="600">
      <br>
    <b>Performance par CANAL de VENTE</b>
  </p>
  <br>
  <b><h2>DASHBOARD</h2></b>
  Bienvenu sur votre espace de pilotage. Cet outil a été conçu pour offrir une <b>visibilité complète</b> sur nos opérations en cours. On a utiliser des filtres pour affiner nos données et optimiser notre flux de travail.<br>
  ces deux figures nous montre l'interface principale de ce tableau de bord.<br>
  <br>
  <table align="center">
      <tr>
          <td align="center">
              <img src="Images\Dashboard1.png" width="300">
            <br>
            <b>Tableau donnant les infos sur l'année 2024 </b>
          </td>
          <td align="center">
            <img src="Images\Dashboard2.png" width="300">
            <br>
            <b>Partie basse de l'interface montrant les performance des diffrents segment sur l'année 2024</b>
          </td>
      </tr>
  </table>
      </tr>
  <br>
  Les segments <b>Années</b> et <b>Regions</b> placés à gauche de la première image rendent le tableau de bord interactif car en choisissant (cliquant) sur une de leur valeur on obtient un chagement imédiat des données du tableau ce qui le rend intéractif. prenons l'exemple de l'année 2025 et regardons les resultats:<br>
  <table align="center">
    <tr>
      <td align="center">
          <img src="Images\Dashboard3.png" width="300">
          <br>
        <b>Image montrant la sélection 2025</b>
      </td>
      <td align="center">
        <img src="Images\Dashboard4.png" width="300">
        <br>
        <b>image montrant les KPI de l'année choisi à gauche</b>
      </td>
    </tr>
  </table>
  <br>
  Biensur le tableau de bord nous donne plusieurs autres choix , par exemple si on veut voir les KPI d'une ou plusieurs villes chois sur une ou plusieurs années il suffit de faire la sélection sur le segment des <b>REGIONS</b> à gauche on aura le resultat voulu.<br>
  <br>
J'insère le fichier EXCEL pour permettre de faire l'expérience en temps réel . <br>
  
