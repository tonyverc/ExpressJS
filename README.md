# ExpressJS

Ce repo contient une appli express.js de type "Hello World" pour tester le deploiement.

## Installation en local

```
git clone https://github.com/tonyverc/ExpressJS
cd ExpressJS
npm install
```

### Utilisation

```bash
node app.js
```

[http://localhost:3000](http://localhost:3000)

## Installation sur render.com

prérequis:un compte github.

-(optionnel)Forkez un repository ou créez un nouveau repository sur github si nécessaire
-créez un compte sur [https://render.com](https://render.com)
-créez un nouveau web service en cliquant sur l'icone « + »
-choisissez l'option « Build and deploy from a git repository »
-cliquez sur « connect account » dans la section « github » à droite
vous vous retrouvez sur le site de github
-Taper votre mot de passe Github
-Selectionnez le repository que vous voulez publier
-Confirmez les permissions accordées
vous revenez sur le site de render
-Cliquez sur le bouton « connect » du repository que vous voulez publier
-Remplissez le champ avec les données suivantes :

    ```
    General:

Name: [sous-domaine-de-votre-appli]
Region: Frankfurt (EU Central)
Branch: main
Root Directory: <nc>
Build Command: npm install
Start Command: node app.js
Instance Type: Free
    ```

Remplacez `<sous-domaine-de-votre-appli>` par votre nom de domaine de votre appli.
Exemple: `foo`donnera `https://foo.onrender.com`

-validez la configuration puis visitez le lien quand le build est terminé

### Mise à jour sur render.com

-Mettez le code à jour
-Commitez votre code avec `git add`` et `git commit`
-Poussez votre code sur github avec `git push`
-Verifiez que le code est à jour sur render.com