# App e-commerce

**Créer une structure propre pour créer une application type e-commerce**

=========================================================================================

- [ ] la page home doit afficher une sélection de produit, pour l'instant juste un produit aléatoire

- [ ] la page shop affiche tous les produits
chaque produit affichera son titre, son image, sa category

- [ ] la page de détail d'un produit affichera tous les éléments du produit sauf l'id

- [ ] une page d'authentification avec un formulaire pour se connecter, juste un champs "alias"

*Algorithme* :  - lire le fichier
                - créer un middleware qui va lire le fichier pour chaque requête
                - on lit le fichier json et on interprète la donnée avec le module fs et la méthode readFile()
                - créer une fonction middleware qui va lire le fichier sur chaque cycle de request/response

> Pour "sauvegarder" une donnée en transit via un middleware, on mets ça dans res.locals.keyName
> On la récupère via cette même propriété après avoir terminé la fonction middleware et "continuer" dans l'instruction d'origne

>> (Structure déjà créée dans le cours_3 node js intro express ejs)


## Page Admin 

**La page d'authentification devient la page admin.**

A partir de cette page: - afficher tous les produits
                        - ajouter un produit

- [ ] Générer l'id du nouveau produit avec <https://www.npmjs.com/package/uuid>

- [ ] Insérer les données du formulaire dans le fichier déjà présent des produits ne s'aidant de la méthode write file du core module "fs" <https://nodejs.dev/fr/learn/writing-files-with-nodejs/>