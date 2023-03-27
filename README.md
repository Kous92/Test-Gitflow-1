# Test GitHub avec Gitflow

Ce contenu est actuellement mis en place avec le concept Gitflow.

## Les commandes, en mode classique
1. Créez un nouveau repository sur GitHub en utilisant le modèle Gitflow. ✅
2. Clonez le repository sur votre ordinateur. ✅
3. Créez une branche "develop" à partir de la branche principale "master". ✅
```
git checkout -b develop
```
4. Effectuez une modification mineure dans un fichier quelconque sur la branche "develop". ✅
5. Ajoutez et validez les modifications, puis fusionnez la branche "develop" dans la branche "master".  ✅
```
git add .
git commit -m "Première modification mineure"
git checkout develop
```
6. Créez une branche "feature" à partir de la branche "develop". ✅
```
git checkout -b feature
```
7. Effectuez une modification significative dans un fichier quelconque sur la branche "feature". ✅
8. Ajoutez et validez les modifications, puis fusionnez la branche "feature" dans la branche "develop". ✅
```
git add .
git commit -m "Première feature"
git checkout develop
git merge feature
```
9. Créez une autre branche "feature2" à partir de la branche "develop". ✅
```
git checkout -b feature2
```
10. Effectuez une modification dans un fichier quelconque sur la branche "feature2". ✅
11. Ajoutez et validez les modifications, puis fusionnez la branche "feature2" dans la branche "develop". ✅
```
git add .
git commit -m "Feature n°2"
git checkout develop
git merge feature2
```
12. Supprimez les branches "feature" et "feature2". ✅
```
git branch -D feature
git branch -D feature2
```
13. Créez une branche "release" à partir de la branche "develop". ✅
```
git checkout -b release
```
14. Effectuez une modification mineure pour préparer la version de la branche "release". ✅
15. Ajoutez et validez les modifications, puis fusionnez la branche "release" dans la branche "main". ✅
```
git add .
git commit -m "Première release"
git checkout main
git merge release
git checkout develop
git merge release
```
16. Créez une étiquette pour la version de la branche "master". 
```
git tag '0.1.0'
```
17. Supprimez la branche "release". ✅
```
git branch -D release
```
18. Vous avez terminé! ✅