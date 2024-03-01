# Principes SOLID Expliqués

Les principes SOLID sont des concepts clés en conception orientée objet qui visent à rendre le code plus maintenable, flexible et évolutif. Voici un résumé de chacun des cinq principes avec des exemples de mauvaises et bonnes pratiques.

## 1. Single Responsibility Principle (SRP)

**Mauvaise pratique :** Une classe `Employe` qui gère à la fois les données des employés et les opérations de base de données.

**Bonne pratique :** Séparer les responsabilités en deux classes : une classe `Employe` pour les données des employés, et une classe `GestionEmploye` pour les opérations de base de données.

## 2. Open/Closed Principle (OCP)

**Mauvaise pratique :** Modifier la classe `Filtre` chaque fois que vous souhaitez ajouter un nouveau critère de filtrage.

**Bonne pratique :** Utiliser des spécifications pour étendre les capacités de filtrage sans modifier la classe `Filtre` existante.

## 3. Liskov Substitution Principle (LSP)

**Mauvaise pratique :** Une classe dérivée `Autruche` de `Oiseau` qui ne peut pas utiliser la méthode `voler` de façon significative.

**Bonne pratique :** Séparer les oiseaux qui volent et ceux qui ne volent pas en différentes hiérarchies pour respecter le LSP.

## 4. Interface Segregation Principle (ISP)

**Mauvaise pratique :** Une interface `Machine` qui oblige les implémenteurs à dépendre de méthodes qu'ils n'utilisent pas.

**Bonne pratique :** Créer des interfaces spécifiques pour que les classes n'aient à implémenter que les méthodes qu'elles utilisent.

## 5. Dependency Inversion Principle (DIP)

**Mauvaise pratique :** Une classe `Interrupteur` dépend directement d'une classe `Lampe` de bas niveau.

**Bonne pratique :** Utiliser des abstractions pour inverser la dépendance, permettant à `Interrupteur` de fonctionner avec n'importe quel dispositif implémentant l'interface `DispositifElectrique`.
