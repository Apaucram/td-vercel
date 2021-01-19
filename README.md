### 4. [CLI] installez et affichez la version de vercel installé sur votre machine
npm i -g vercel
vercel --version

### 5. [CLI] créez un nouveau projet sur votre machine
Installation du cli angular :
npm i -g @angular/cli
Initialisation du projet :
ng new app

### 6. [CLI] déployer l'application dans vercel
dans le dossier racine :
vercel

### 7.  [CLI] lister les différents déploiements qui ont eu lieu sur votre projet
vercel ls

###8.  [CLI] afficher les logs liés au déploiement précédent
On utilise la commande :
vercel logs [deployment-url]
dans notre cas :
vercel logs https://td-vercel-ivory.vercel.app

### 9.  [CLI] Utilisez la commande inspect
La commande vercel inspect est utilisée pour récupérer des informations sur un déploiement
vercel inspect https://td-vercel-ivory.vercel.app

### 10. Variables d'environnement
Selon la documentation :
Environment Variables are accessible during both the Build Step and Runtime and can be configured for Production, Preview, and Development Environments individually.

This allows you to inject values that you don't want to place directly in your source code and change its behavior depending on the Environment its running in.


### 11.  [CLI] créer une variable d'evironnement
vercel env add


### 12.  [CLI] lister les variables d'environnement sur votre projet
vercel env ls


### 13. Les secrets
La variable est chiffré pour ne pas etre stocker en clair


### 15. [CLI] Créez une variable d'env de type secret
vercel env add
vercel secret add pass toto123

### 16. Environnements
Listez les trois environnements que met automatiquement Vercel à notre disposition pour un meme projet
​Production Preview Development

Pourquoi plusieurs environnements pour un meme projet ? Quel en est l'utilité dans un projet ? 
L'environement de developpement est utiliser pour le développement, c'est à dire que les que toutes les fonctionalitées ne sont pas totalement implémentés. Production correspond à la version stable.
L'environnement de preview sert pour réaliser une dernière vérification de notre application juste avant la mise en production.






