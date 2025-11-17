<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

  <p align="center">A progressive <a href="http://nodejs.org" target="_blank">Node.js</a> framework for building efficient and scalable server-side applications.</p>
    <p align="center">
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/dm/@nestjs/common.svg" alt="NPM Downloads" /></a>
<a href="https://circleci.com/gh/nestjs/nest" target="_blank"><img src="https://img.shields.io/circleci/build/github/nestjs/nest/master" alt="CircleCI" /></a>
<a href="https://coveralls.io/github/nestjs/nest?branch=master" target="_blank"><img src="https://coveralls.io/repos/github/nestjs/nest/badge.svg?branch=master#9" alt="Coverage" /></a>
<a href="https://discord.gg/G7Qnnhy" target="_blank"><img src="https://img.shields.io/badge/discord-online-brightgreen.svg" alt="Discord"/></a>
<a href="https://opencollective.com/nest#backer" target="_blank"><img src="https://opencollective.com/nest/backers/badge.svg" alt="Backers on Open Collective" /></a>
<a href="https://opencollective.com/nest#sponsor" target="_blank"><img src="https://opencollective.com/nest/sponsors/badge.svg" alt="Sponsors on Open Collective" /></a>
  <a href="https://paypal.me/kamilmysliwiec" target="_blank"><img src="https://img.shields.io/badge/Donate-PayPal-ff3f59.svg" alt="Donate us"/></a>
    <a href="https://opencollective.com/nest#sponsor"  target="_blank"><img src="https://img.shields.io/badge/Support%20us-Open%20Collective-41B883.svg" alt="Support us"></a>
  <a href="https://twitter.com/nestframework" target="_blank"><img src="https://img.shields.io/twitter/follow/nestframework.svg?style=social&label=Follow" alt="Follow us on Twitter"></a>
</p>
  <!--[![Backers on Open Collective](https://opencollective.com/nest/backers/badge.svg)](https://opencollective.com/nest#backer)
  [![Sponsors on Open Collective](https://opencollective.com/nest/sponsors/badge.svg)](https://opencollective.com/nest#sponsor)-->

# Login API

Login API est une application serveur scalable et efficace construite avec le framework [NestJS](https://nestjs.com). Elle fournit une plateforme robuste pour la gestion des utilisateurs et l'authentification via tokens JWT.

## Fonctionnalités

### Gestion des Utilisateurs
- **Inscription**: Permet aux utilisateurs de créer un compte avec des mots de passe sécurisés via bcrypt.
- **Connexion**: Authentifie les utilisateurs via email et mot de passe, délivrant des tokens JWT (access et refresh tokens) lors d'une connexion réussie.
- **Gestion des Tokens**: 
  - Tokens d'accès pour l'authentification à court terme.
  - Tokens de rafraîchissement pour obtenir de nouveaux tokens d'accès sans ré-authentification.
- **Autorisation**: Protège les routes en utilisant des guards pour s'assurer que seuls les utilisateurs authentifiés peuvent accéder à des endpoints spécifiques.

### Configuration de l'Environnement
- Utilise des variables d'environnement pour gérer les configurations sensibles comme les URIs de base de données, les secrets JWT, et les durées d'expiration des tokens.
- Configuration centralisée assurant flexibilité et sécurité lors du déploiement.

## Project Setup

```bash
$ npm install
```

## Compile and run the project

```bash
# development
$ npm run st
# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Run tests

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Ressources

Consultez quelques ressources qui peuvent être utiles lors du travail avec NestJS:

- Visitez la [Documentation NestJS](https://docs.nestjs.com) pour en savoir plus sur le framework.

## Variables d'Environnement

Pour configurer votre application, définissez les variables d'environnement suivantes:

```plaintext
DB_URI=mongodb://localhost:27017/login-api
JWT_SECRET=your_jwt_secret
JWT_ACCESS_TOKEN_EXPIRES=3600s
JWT_REFRESH_TOKEN_SECRET=your_refresh_token_secret
JWT_REFRESH_TOKEN_EXPIRES=7d
```

## Support

Nest est un projet open source sous licence MIT. Il peut grandir grâce aux sponsors et au soutien des incroyables contributeurs. Si vous souhaitez les rejoindre, veuillez [lire plus ici](https://docs.nestjs.com/support).

## Contact

- Project Manager - [Linerol TCHECOUNNOU](sessiessenamlinerol.tchecounnou@ynov.com)
- Backend Developer - [Jenny CHOUFACK](jenny.choufack@ynov.com)
- Backend Developer - [Hanim MOUSSA YARI](hanimorounassara.moussayari@ynov.com)

## License

Nest is [MIT licensed](https://github.com/nestjs/nest/blob/master/LICENSE).
