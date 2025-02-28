## Questions ouvertes

### Décrivez les étapes pour créer un Service Account dans GCP. Quelles sont les bonnes pratiques à suivre en matière de gestion des clés et de sécurité ?

Les étapes sont les suivantes :
se rendre dans IAM et administration > Comptes de service > + créer un compte de service

Il faut ensuite lui donner un nom, donner les droits au compte de service et donner les droits d'utiliser ce compte de service.

Pour les bonnes pratiques il faut eviter la fuite d'identifiants, mettre en place seulement les droits nécessaires pour éviter que le compte ne soit utiliser à d'autres fins.


### Comment créer un bucket sur Google Cloud Storage ? Précisez les configurations importantes à définir (localisation, politique de conservation, etc.) et comment celles-ci impactent la sécurité et la performance.

Sur GCP se rendre dans Clourd storage > Buckets > + créer

Ensuite il faut donner un nom, le lieu de stockage, les droits d'accées. 

Les configurations sur la localisation permettent un accés plus rapide aux données ainsi que de respectés les eventuelles legislations en termes de conservation des données (RGPD par exemple), la politique de conservation va influer sur la sécurité des données sur le point de vue conservations. On peut chosir du dupliquer sur plusisieurs endroits les données pour éviter les pertes.


###  En quoi consiste la gestion des identités et des accès (IAM) sur GCP ? Donnez un exemple concret de configuration des droits pour limiter l'accès à une ressource critique.

On peut autoriser et refuser l'accés à certaines fonctionnalités et données de gcp. Par exemple on ne va donner l'accées à la facturation qu'au service comptabilité d'une entreprise pour éviter qu'elle ne face des bétises donc la configuration des machines virtuelles et buckets.


### Expliquez comment configurer la facturation sur GCP. Quelles précautions recommanderiez-vous pour éviter des coûts imprévus lors du déploiement de projets ?

Dans l'onglet facturation nous pouvons créer des budgets avec alertes. Il est facile d'augmenter la facture si on ne regarde pas les choix que l'on fait. C'est pourquoi créer un budget va nous permettre de fixer une limite et dêtre avertis quand la moitié, 3/4, la totalité du budget sera atteint.

### Quelle est la chose importante que l'on dit à la fin du cours en quittant la salle de TP ?

au revoir et merci pour ce cours haha !!

