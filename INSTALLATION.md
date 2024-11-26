# Installation Cypress 💻

Bienvenue dans cette section d'installation de **Cypress** ! Nous allons détailler les étapes pour installer Cypress, adaptées à votre système d'exploitation, que vous soyez sur Windows, macOS, ou Linux. Suivez les instructions pour préparer votre environnement de développement, et vous serez prêt à écrire vos premiers tests en un rien de temps.

---

### 1. Préparer l’Environnement 🛠️

Avant d'installer Cypress, assurez-vous d'avoir déjà installé **Node.js** et **npm** (Node Package Manager). Vous pouvez vérifier si Node.js est installé en exécutant la commande suivante dans votre terminal :

```bash
node -v
```

Si cela renvoie une version, alors Node.js est prêt. Sinon, téléchargez-le depuis [nodejs.org](https://nodejs.org/). Une fois Node.js installé, npm sera également installé automatiquement.

### 2. Installation de Cypress 🚀

#### Étape 1 : Ouvrir le Terminal (ou l’Invite de Commandes)

- **Windows** : Recherchez "Invite de commandes" ou ouvrez **PowerShell**.
- **macOS** : Utilisez l’application **Terminal**.
- **Linux** : Utilisez votre **terminal préféré** (ex. GNOME Terminal, Konsole, etc.).

#### Étape 2 : Naviguer vers votre Dossier de Projet

Dans le terminal, utilisez la commande `cd` pour vous déplacer vers le dossier de votre projet où vous souhaitez installer Cypress. Si vous n'avez pas encore créer votre dossier de projet, créez un et copiez le chemin.

```bash
cd D:/mon_premier_test
```

#### Étape 3 : Installer Cypress avec npm

Une fois dans le dossier de votre projet, lancez la commande suivante pour créer un package.json dans votre dossier:

```bash
npm init -y
```

Après vous tapez le commande suivante pour installer Cypress en tant que dépendance :

```bash
npm install cypress --save-dev
```

> **Note** : L'option `--save-dev` ajoute Cypress en tant que dépendance de développement, ce qui signifie qu'il sera utilisé uniquement pendant la phase de développement.

### 3. Vérifier l’Installation ✅

Après l'installation, vous pouvez vérifier que Cypress est bien installé en le lançant directement avec la commande suivante :

```bash
npx cypress open
```

Cette commande ouvre l’interface graphique de Cypress, vous permettant de configurer vos premiers tests.

---

### 4. Instructions Spécifiques par Système d'Exploitation 🖥️

#### Windows

- **Permissions d’Administrateur** : Assurez-vous d’exécuter l’installation avec les droits d’administrateur si nécessaire.
- **Installation avec PowerShell** : Si vous rencontrez des problèmes d'installation, exécutez PowerShell en mode administrateur et essayez de réinstaller avec `npm install cypress --save-dev`. Si le problème persiste, utilisez d'autre terminal comme **cmd** ou **Git bash**

#### macOS

- **Permissions de Sécurité** : macOS peut vous demander des autorisations pour accéder à certains fichiers. Si vous recevez une alerte de sécurité lors de l'ouverture de Cypress, allez dans **Préférences Système > Sécurité et confidentialité** pour autoriser l'application.

#### Linux

- **Dépendances LibX11** : Certaines distributions Linux peuvent nécessiter l'installation de bibliothèques supplémentaires pour Cypress. Sur Debian/Ubuntu, par exemple, exécutez cette commande si Cypress ne s’ouvre pas correctement :
    
    ```bash
    sudo apt-get install libx11-xcb1 libasound2
    ```
    
- **Exécution en Root** : Si vous travaillez avec des droits root, utilisez l’option `--no-sandbox` pour éviter les erreurs liées aux permissions :
    
    ```bash
    npx cypress open --no-sandbox
    ```
    

---

### Cypress est Prêt 🎉

Une fois Cypress ouvert, vous êtes prêt pour la suite ! Dans la prochaine section, nous allons voir comment configurer votre premier test Cypress et parcourir l'interface.

__Prochaine étape :__ [Configuration de Cypress ⚙️](/CONFIGURATION.md)
