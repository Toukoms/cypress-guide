# Configuration de Cypress ⚙️

Maintenant que Cypress est installé, configurons-le pour qu'il fonctionne de manière optimale avec votre projet. Suivez ces étapes pour initialiser la configuration de Cypress et explorer les paramètres de base qui vous permettront de personnaliser votre environnement de test.

---

### 1. Lancement de Cypress et Accès au Launchpad 🚀

Lorsque vous ouvrez Cypress pour la première fois avec la commande suivante :

```bash
npx cypress open
```

Cypress va démarrer et afficher une interface appelée le **Launchpad**. Cet outil vous guide à travers toutes les étapes de configuration nécessaires avant de pouvoir écrire votre premier test.

---

### 2. Choix du Type de Test 🔍

La première étape consiste à choisir le **type de test** que vous souhaitez exécuter :

- **E2E Testing (Test de bout en bout)** : Pour tester l'application dans son ensemble en naviguant entre les pages et en simulant des interactions utilisateur.
- **Component Testing (Test de composant)** : Pour tester des composants individuels en les montant dans un environnement isolé.

Si vous débutez avec Cypress ou que vous n'êtes pas certain du type de test à choisir, sélectionnez **E2E Testing**. Vous pourrez toujours changer de type de test plus tard si nécessaire.

---

### 3. Configuration Rapide 📝

Après avoir sélectionné le type de test, le Launchpad configure automatiquement Cypress pour votre projet en créant les fichiers de configuration adaptés. Voici les éléments que Cypress va créer :

- Dossier `cypress` avec une structure organisée pour vos fichiers de tests, fixtures et commandes personnalisées.
- Fichier de configuration (`cypress.config.js` ou `cypress.config.ts`) contenant les paramètres de base de Cypress pour le projet.

Le Launchpad vous présentera une liste de tous les fichiers générés pour votre révision. Vous pouvez cliquer sur **Continue** pour accepter la configuration par défaut et passer à l'étape suivante.

---

### 4. Sélection du Navigateur 🌐

Enfin, Cypress détecte automatiquement les navigateurs compatibles installés sur votre système et vous présente une liste pour choisir celui que vous souhaitez utiliser pour vos tests. Cypress prend en charge plusieurs navigateurs populaires, et vous pouvez en changer à tout moment selon vos préférences ou les besoins de votre projet.

Une fois votre choix effectué, cliquez sur **Start** pour démarrer le navigateur sélectionné.

---

### Cypress est Configuré 🎉

Vous avez maintenant configuré Cypress et êtes prêt à démarrer votre aventure de test ! Grâce au Launchpad, toutes les étapes de configuration ont été guidées et automatisées pour que vous puissiez commencer vos premiers tests en quelques clics. Dans la prochaine section, nous aborderons comment écrire et structurer vos premiers tests avec Cypress.

__Prochaine étape :__ [[Premier test en Cypress🚀]]
