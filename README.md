# INSTALLATION

#### DataBase

- Démarrer le serveur MySQL
- Créer une base de donnée "**groupomania**" ( ou n'importe quel autre nom, celui-ci sera renseigné dans _.env_ )
- Créer un utilisateur en notant bien son **nom**, son **mot de passe** et sa **clé secrête** ( cette dernière peut être identique au mot de passe )
- Créer un fichier **.env** dans le dossier _./backend_ et le renseigner avec les données précédentes au format suivant :
  - HOST = localhost
  - DATABASE = **groupomania**
  - DB_USERNAME = **nom**
  - DB_PASSWORD = **mot de passe**
  - PORT = 3000
  - SECRET_KEY = **clé secrête**
  - ACCESS_TOKEN = **token** ( afin d'obtenir un token il est possible de rentrer dans la console `node` puis `require(crypto).randomBytes(64).toString('hex')` et de copier la chaîne de caractères ainsi obtenue )

_FACULTATIF_

- Importer "groupomania.sql" inclus à la racine du fichier dans la base de donnée, les identifiants des utilisateurs enregistrés dans cette DB sont :
  - email: kuai@liang.mk, password: adminaccount, role: admin
  - email: john@doe.com, password: azerty1, role: employee
  - email: jane@doe.com, password: azerty1, role: employee

#### Backend

- Se positionner dans le dossier _./backend_
- Puis lancer la commande `npm install`
- Ensuite `nodemon server`
- Le message _"Connection has been established successfully."_ doit s'afficher dans la console ainsi que la creation de la _DB_

#### Frontend

- Se positionner dans le dossier _./frontend_
- Puis lancer la commande `npm install`
- Ensuite `npm run serve`
- Depuis le navigateur web, se rendre à l'adresse indiquée en local (par défaut: http://localhost:8080/)
