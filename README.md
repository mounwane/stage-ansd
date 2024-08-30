# stage-ansd
Modèles de prédiction de rendements

Ce github a été créé pour répertorier les fichiers qui ont eu a être créés dans le cadre du stage de Mountaga Wane à l'ANSD sur la prédiction de rendements à partir notamment de données issues d'images satellites.

Remarque: Les données satellites utilisées lors du travail préliminaire d'affichage de cartes ndvi n'ont pas pu être chargées car trop volumineuses. Elles sont disponibles en libre service sur Copernicus: [https://land.copernicus.eu/en](https://browser.dataspace.copernicus.eu/?zoom=5&lat=50.16282&lng=20.78613&themeId=DEFAULT-THEME&datasetId=S2_L2A_CDAS&demSource3D=%22MAPZEN%22&cloudCoverage=30&dateMode=SINGLE)

Le notebook stage_ansd correspond aux premiers travaux d'extraction de données satellites que j'ai eus à réaliser. Il s'agissait notamment de se faire la main et d'exploiter les indices NDVI sur les parcelles.

Le notebook notebook_principal correspond au travail principal que j'ai eu à réaliser. Celui-ci concerne l'estimation des productions agricoles par département au Sénégal. Nous avons d'abord travaillé dans un premier temps sur l'arachide avant d'étendre nos modèles à d'autres cultures telles que le sorgho et le riz. Pour ce dernier, il a fallu décortiquer le modèle afin d'avoir de meilleures performances, notamment parce que plusieurs départements n'en produisent pas. Par la suite, il a également fallu ré-ajuster la fonction de perte car le modèle avait tendance à sous-évaluer les prédictions.

Le notebook notebook_geomaticien correspond aux premiers travaux d'extraction que j'ai eu à faire avec les données de la DAPSA. Celà s'est notamment fait en utilisant Google Earth Engine afin de tirer les indices satellites souhaités. Ce notebook pourra également servir de base de test, non exhaustive bien sûr, pour le recrutement de géomaticiens en cours.
