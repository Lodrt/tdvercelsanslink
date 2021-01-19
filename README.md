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




























![Angular Logo](https://github.com/vercel/vercel/blob/master/packages/frameworks/logos/angular.svg)

# Angular Example

This directory is a brief example of an [Angular](https://angular.io/) app that can be deployed with Vercel and zero configuration.

## Deploy Your Own

Deploy your own Angular project with Vercel.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/vercel/vercel/tree/master/examples/angular)

_Live Example: https://angular.now-examples.now.sh_

### How We Created This Example

To get started with Angular, you can use the [Angular CLI](https://cli.angular.io/) to initialize the project:

```shell
$ ng new
```
