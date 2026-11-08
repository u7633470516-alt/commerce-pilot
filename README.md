# Commerce Pilot

Un logiciel e-commerce autonome pour simuler la rentabilité de tes produits.

## Démarrage
1. Clique sur **Code → Download ZIP** et décompresse le dossier.
2. Ouvre **index.html** dans Chrome, Firefox ou Edge récent.
3. Renseigne tes coûts puis enregistre tes produits.

Aucune installation, dépendance ou clé API nécessaire.

## Fonctionnalités
- Calcul de marge par commande, CPA maximum et ROAS minimum.
- Projection du chiffre d’affaires et du bénéfice selon le nombre de commandes.
- Catalogue avec recherche et modification des produits.
- Sauvegarde locale dans le navigateur et export CSV.
- EUR, USD et GBP ; montants saisis dans une seule devise par produit.
- Interface responsive en français.

## Calculs
Marge avant publicité = prix HT − fournisseur − livraison − autres coûts − frais fixes par commande − frais de paiement.

Bénéfice par commande = marge avant publicité − CPA.

ROAS minimum = prix HT / marge avant publicité (impossible si cette marge est nulle ou négative).

Exemple : prix 59,90 ; fournisseur 15 ; livraison 5 ; frais 2,9 % + 0,30 ; CPA 15 → bénéfice estimé 22,8629 par commande.

## Données et limites
Les données restent dans le stockage du navigateur : pas de synchronisation, serveur ou connexion Shopify. Exporte régulièrement le CSV. Effacer les données du navigateur supprime le catalogue local. Le CSV est un export ; l’import n’est pas disponible dans cette version.

Les estimations sont avant impôts et charges fixes. Intègre les remises, retours et autres dépenses pour affiner les simulations. Aucun taux fiscal n’est automatiquement appliqué.

## Validation
Syntaxe JavaScript vérifiée et trois scénarios de calcul validés : marge positive, coût supérieur au prix et publicité déficitaire. Les parcours complets de l’interface restent à tester dans le navigateur.

## Suite du projet
- Import CSV et sauvegarde JSON.
- Tableau de bord des commandes réelles.
- Connexion Shopify après configuration et autorisation de la boutique.
