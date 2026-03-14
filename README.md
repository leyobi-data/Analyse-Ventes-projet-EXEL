# Analyse-Ventes-projet-EXEL
<br>
<b><h2> 📊Optimisation des performance commerciale: Analyse de données de Ventes( Excel & Power Query)<h2></h2></b><br>
<br>
Dans le cadre d'une simulation d'entretien pour le poste de <b>Data Analyst</b>, j'ai été chargé d'accompagner une Entreprise de distribution d'équipements technologique dans l'analyse de ses performances pluriannuelles.<br>
<br>
Face à un jeu de données brut de <b>1000 transactions</b>, l'enjeu était double: assainir une structure de données complexe et transformer ces chiffres en <b>indicateurs de performance</b> actionnables. Ce projet démontre ma capcité à gérer l'intégralité du cycle de donnée de l'ingestion via <b>Power Query</b> à la création de <b>Dashboards intéractifs</b> pour répondre à une problématique de croissance commerciale.<br>
<p align="center">
  <img src="Images\Données_Brutes.png" alt="Vu Exel" width="600">
    <br>
      <b>Image de données Brut via Excel</b>
</p>
<br>
<b><h2>Etape 1: Audit et Préparation des Données (Power Query></h2></b><br>
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
  <p align="center">
    <img src="Images\P_Qwery_Type_de_données.png" alt="Transformation Power Query" width="400">
    <img src="Images\New_Table_after_PowerQuery.png" alt="after Power Query" width="400">
      <br>
  </p>
  <br>
  
