---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-01"

---

{:new_window: target="_blank"}  
{:shortdesc: .shortdesc}


# Ajout de nouvelles données d'identification du service
{: #service_credentials}

Vous pouvez générer un nouveau jeu de données d'identification de service au cas où vous voudriez connecter manuellement un consommateur extérieur à un service Bluemix. Par exemple, si vous tentez de lier une application AWS à un service Watson, vous devrez générer de nouvelles données d'identification du service pouvant être utilisées pour lier entre-eux ces deux services.

Les services Cloud Foundry peuvent générer une clé de service, également dénommée données d'identification du service. Ces données sont spécifiques au service concerné et varient en fonction de la manière dont chaque service définit les données d'identification devant être générées. Ces données d'identification peuvent contenir un nom d'utilisateur, un mot de passe, un nom d'hôte et une URL. Toutefois, le contenu de chaque donnée d'identification du service est unique au service qui le génère. Certains services peuvent générer des données supplémentaires nécessitant de renseigner des paramètres. Par exemple, un service peut vous demander d'entrer un paramètre langue pour définir la langue par défaut dans clé de service générée. 

Pour ajouter de nouvelles données d'identification de service, procédez comme suit :

1. Dans la page des détails du service, sélectionnez l'onglet Données d'identification pour le service et cliquez sur **Nouvelles données d'identification + **.
2. Dans la boîte de dialogue Ajouter de nouvelles données d'identification, entrez un **Nom**.
3. Vous pouvez également fournir d'autres paramètres par le biais d'un objet JSON valide contenant des paramètres de configuration spécifiques au service et qui seront soumises soit en ligne, soit dans un fichier.

  **Remarque **. La plupart des services ne requièrent pas de paramètres supplémentaires et pour ceux qui en ont besoin, chaque service définit sa propre liste unique de paramètres. Pour la liste des paramètres de configuration pris en charge, reportez-vous à la documentation de l'offre de service concernée.
4. Cliquez sur **Ajouter** pour générer les nouvelles données d'identification du service.
