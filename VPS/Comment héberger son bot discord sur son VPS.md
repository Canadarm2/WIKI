Dans cet article, vous apprendrez comment héberger votre bot discord sur votre vps.

**Si node.js n'est pas installé, vous devez l'installer!**
Dans un premier temps, connectez vous en **SFTP** et importez votre bot. S'il n'y a pas de package.json, faites la commande suivante: `cd le-dossier-de-votre-bot && npm init
Veuillez bien remplacer le-dossier-de-votre-bot par le dossier de votre bot! 😊
Dans un deuxième temps, installez le module pm2: `npm install --global pm2`
Pour vous assurer si vos modules sont à jours, faites: `npm install -g`
Ensuite, place au démarrage! `pm2 start --name "nom-de-bot" principal.js`
Remplacez principal par le nom de votre fichier principal et nom-de-bot par un nom de bot.
Puis faites `pm2 log`; si ça génère une erreur, supprimez votre dossier node modules et faire `npm ci`.
J'espère que cet article vous aura aidé!