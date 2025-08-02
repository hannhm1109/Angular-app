# Interface de Gestion de Produits Angular

Cette application Angular présente une interface simple pour la consultation et la gestion d'une collection de produits via un backend Spring Boot.

## Fonctionnalités principales

- Affichage de la liste des produits avec identifiant, nom, prix et statut de sélection
- Suppression de produits avec demande de confirmation
- Mise à jour automatique de la liste après suppression
- Consommation d'API REST pour les opérations backend
- Interface utilisateur enrichie avec des icônes Bootstrap

## Technologies utilisées

- Angular 16+
- TypeScript
- Bootstrap Icons
- RxJS et HttpClient
- API RESTful Spring Boot

## Configuration du backend

Cette interface se connecte au dépôt backend maintenu par **[Dr. Mohamed Youssfi](https://github.com/mohamedYoussfi/products-service)**.

- URL de base de l'API : `http://localhost:8083`
- Point d'accès produits : `/products`

Assurez-vous de démarrer le service :
```bash
cd products-service
mvn spring-boot:run
```
> Le backend doit fonctionner sur le port `8083` pour que cette interface soit opérationnelle.

## Lancement de l'application en local

### 1. Cloner le projet et installer les dépendances

```bash
git clone https://github.com/saadBr/ang-app.git
cd ang-app
npm install
```

### 2. Démarrer le serveur de développement

```bash
ng serve
```

Accédez ensuite à : [http://localhost:4200/products](http://localhost:4200/products)

## Architecture de l'application

```
src/
├── app/
│   ├── products/
│   │   ├── products.ts        # Logique du composant
│   │   ├── products.html      # Template de vue
│   │   └── products.css       # Styles du composant
│   ├── services/
│   │   └── products.ts        # ProductService (appels API)
│   └── app.routes.ts          # Configuration des routes
```

## Licence

Usage éducatif uniquement. Basé sur les travaux dirigés de Mohamed Youssfi.