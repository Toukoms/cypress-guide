# Premier test en Cypress🚀.md

Pour votre premier test, nous allons utiliser Cypress pour visiter une page web et vérifier que le texte "Bienvenue" est présent. Ce test simple vous permettra de vous familiariser avec les commandes de base de Cypress et d’observer comment il interagit avec une page web.

### Étape 1 : Créer le Test 📄

Pour commencer, dans votre projet Cypress, créez un fichier de test dans le dossier `cypress/e2e`. Nommez ce fichier `premier_test.cy.js`.

### Étape 2 : Écrire le Test ✅

Dans ce fichier, ajoutez le code suivant :

```javascript
describe('Visite du site et vérification du texte de bienvenue', () => {
	it('Doit afficher le texte Bienvenue sur la page', () => {
		// 1. Visiter le site web
		cy.visit('https://odyssee.vivetic.com');
		// 2. Vérifier que le texte "Bienvenue" est présent dans la page
		cy.contains('Bienvenue').should('be.visible');
	});
});
```

---

### Explication du Code 📘

Voyons maintenant en détail le rôle de chaque ligne de code :

- **`describe()`** : Il s'agit d'une fonction permettant de regrouper plusieurs tests similaires sous un même nom. Ici, nous donnons au groupe de tests le titre "Visite du site et vérification du texte de bienvenue".
    
- **`it()`** : Cette fonction est utilisée pour définir un test individuel. Le nom que vous lui donnez décrit précisément ce que le test est censé vérifier. Dans ce cas, nous décrivons notre test comme "Doit afficher le texte Bienvenue sur la page".
    
- **`cy.visit('https://odyssee.vivetic.com');`** : La commande `cy.visit()` dit à Cypress d'ouvrir la page à l'URL spécifiée. Ici, nous lui demandons d'ouvrir la page `https://odyssee.vivetic.com`.
    
- **`cy.contains('Bienvenue').should('be.visible');`** : Cette ligne utilise deux commandes :
    
    - `cy.contains('Bienvenue')` cherche le texte "Bienvenue" sur la page.
    - `.should('be.visible')` vérifie que cet élément contenant "Bienvenue" est bien visible à l'écran.

---

### Exécuter le Test ▶️

Pour exécuter ce test, ouvrez le terminal et relancez Cypress avec la commande suivante (si Cypress n’est pas encore ouvert) :

```bash
npx cypress open
```

Ensuite, sélectionnez votre fichier `premier_test.cy.js` dans l’interface de Cypress pour l'exécuter. Cypress ouvrira un navigateur et montrera visuellement chaque étape du test.

---

### Pour Aller Plus Loin 🔗

Vous trouverez dans le fichier d’aide en Markdown une liste des **commandes fréquemment utilisées** pour le test end-to-end, comme :

- **`cy.visit()`** : Pour naviguer vers une page web.
- **`cy.contains()`** : Pour rechercher un texte spécifique dans la page.
- **`cy.get()`** : Pour sélectionner des éléments en utilisant des sélecteurs CSS.
- **`should()`** : Pour faire des assertions et vérifier l’état d’un élément ou d’une commande.

Ces commandes vous seront très utiles pour écrire des tests plus complets. Ce fichier Markdown de "cheat sheet" vous servira de référence pour les commandes courantes à utiliser dans vos tests end-to-end.

---

### Bravo, Vous Avez Écrit Votre Premier Test Cypress ! 🎉

Ce premier test vous donne une bonne base pour interagir avec une page et vérifier des éléments. Dans la prochaine étape, nous explorerons comment interagir avec des éléments plus complexes, comme des formulaires et des boutons, pour créer des tests plus avancés.
