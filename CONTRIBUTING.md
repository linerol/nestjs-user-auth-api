# Contributing Guide

Merci de votre intérêt pour ce template ! Voici comment contribuer.

## Pour les utilisateurs du template

### 1. **Créer un nouveau repository depuis ce template**
   - Sur GitHub, cliquez sur **"Use this template"** → **"Create a new repository"**
   - Choisissez un nom pour votre projet
   - Clonez le nouveau repository

### 2. **Configuration initiale**
   ```bash
   npm install
   cp .env.example .env
   # Mettez à jour les variables dans .env
   ```

### 3. **Démarrer le développement**
   ```bash
   npm run start:dev
   ```

### 4. **Personnaliser pour votre projet**
   - Mettez à jour `package.json` (name, description, author)
   - Modifiez le `README.md` pour votre projet
   - Adaptez la structure des modules selon vos besoins
   - Changez les secrets JWT dans `.env`

## Pour les contributeurs du template

### Signaler des bugs
- Créez une issue avec le label `bug`
- Décrivez le comportement observé et attendu
- Incluez les étapes pour reproduire

### Proposer des améliorations
- Créez une issue avec le label `enhancement`
- Expliquez votre proposition
- Attendez le feedback avant de commencer le développement

### Pull Requests
1. Fork le repository
2. Créez une branche : `git checkout -b feature/your-feature`
3. Commitez vos changements : `git commit -m 'Add new feature'`
4. Poussez la branche : `git push origin feature/your-feature`
5. Ouvrez une Pull Request

## Standards

- Utilisez TypeScript strictement
- Suivez les conventions ESLint du projet
- Écrivez des tests pour les nouvelles fonctionnalités
- Documentez les changements dans le README si nécessaire

## Questions ?

Contactez les mainteneurs du template.
