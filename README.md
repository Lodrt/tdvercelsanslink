q3) npm i -g vercel
q4) vercel -v
q5) vercel init
q6) cd angular then vercel
q7) vercel ls
q8) vercel log angular-es6w6byhk.vercel.app
q9) 
vercel inspect angular-es6w6byhk.vercel.app 
Cette commande permet de voir les informations liées au déploiement du prjet sur vercel notamment les builds, l'url

q10) 

Les variables d'environnement sont des variables en dehors du code source, et qui peuvent donc être modifiées en fonction 
de l'environnement actuellement démarré. 
On peut donc alors facilement avoir des configurations différentes pour les environnements de production,développement ou preview.
Cela permet aussi d'avoir un peu plus de sécurité puisque ces variables ne sont pas dans le code source.

q11) vercel env add plain myVar - > value : question11
q12) vercel env ls  --> liste des variables environnement ( on remarque celle que l'on vient de créer)
q13) Secrets permet de stocker et partager des informations entre déploiements de manière sécurisée car les secrets sont encryptés. 
q14-15) vercel secret add murmure --> pour créer un secret appellé murmure chut ( nom murmure , value chut)
	vercel env add secret testcli production --> pour créer une env var. de type secret appellée testcli 
	Sa valeur est murmure --> le secret créé auparavant 

q16) 3 environnements : production, développement, prévisualisation ( preview) 
      
Cela permet de pouvoir décomposer le travail au sein du projet et donc de pouvoir travailler a plusieurs de manière optimisée

q17) 
q18) https://tdvercelsanslink.vercel.app/ ( PRODUCTION ENV) 
q19) les pull request sont des notifications aux autres membres du projet comme quoi un pull est disponible et nécessaire
     git branch q19 modif readme NOUVELLE BRANCHE 

vercel déploie la pull request dans l'environnement de preview. 

q20) une fois le merge fait, vercel build et dploie le projet dans l'environnement de production

On peut notamment le voir a cette adresse : https://github.com/Lodrt/tdvercelsanslink/deployments

q21) 
L'environnement de production correspond à la branche "master" 

Les pull requests permettent d'appliquer les changements effectués sur le projet dans l'application
mais seulement une fois que les modifications qui ont été faites sur une autre branche ( en preview) sont valides

Le workflow du développement à la production est le suivant : 
	- travail en local sur une branche 
	- developpemnt/ test de la feature
	- commit et push sur github 
	- création d'une pull request 
	- test du merge - > SI OK MERGE 
	- build puis déploiement dans l'environnement de production

q22) tiré de : https://serverless-stack.com/chapters/fr/what-is-serverless.html#:~:text=L'architecture%20serverless%20est%20un,de%20mani%C3%A8re%20dynamique%20les%20ressources.&text=Le%20code%20envoy%C3%A9%20au%20fournisseur,la%20forme%20d'une%20fonction.

architecture serverless est un modèle ou le client va créer son application sur un serveur cloud qui va gérer : 
	les ressources utilisées 
	l'exécution de code ( dans des conteneurs qui vont être trigger avec des events)

Ainsi les fournisseurs de cloud vont seulement récupérer des fonctions lors de l'exécution pour déclencher les conteneurs 
C'est pourquoi on appelle aussi cela FaaS Function as a service 

Les principaux :
AWS ( Amazon Web Service )
AZURE ( Microsoft )
Google Cloud 

q23)







