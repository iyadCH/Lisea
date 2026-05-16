# Lisea 📚

> Application web de suivi de lecture — HTML/CSS/JS pur + Docker/nginx

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![nginx](https://img.shields.io/badge/nginx-009639?style=flat&logo=nginx&logoColor=white)

## 🚀 Lancer avec Docker

```bash
git clone https://github.com/iyadCH/lisea.git
cd lisea
docker compose up --build
```

Ouvre ensuite **http://localhost:3000**

## ⚡ Sans Docker

Ouvre simplement `index.html` dans ton navigateur, ou :

```bash
npx serve .
```

## ✨ Fonctionnalités

- 📚 Bibliothèque avec recherche Open Library (couvertures, auteurs, pages)
- ⏱ Timer de lecture intégré
- 📊 Statistiques avancées + heatmap annuelle
- 🎯 Objectifs annuel, mensuel, hebdomadaire
- ⭐ Notation, tags, notes personnelles
- 🔍 Recherche & tri dans la bibliothèque (Ctrl+K)
- 💾 Persistance localStorage + export/import JSON
- 🌙 Mode sombre/clair
- 📱 Responsive mobile

## 🗂️ Structure

```
lisea/
├── index.html
├── css/
│   ├── base.css          ← variables, reset, typographie
│   ├── layout.css        ← sidebar, app shell, responsive
│   ├── components.css    ← cartes, boutons, formulaires
│   └── pages.css         ← styles spécifiques par page
├── js/
│   ├── state.js          ← localStorage, état global
│   ├── router.js         ← navigation
│   ├── ui.js             ← toast, confirm, thème, helpers
│   ├── books.js          ← bibliothèque + recherche
│   ├── sessions.js       ← timer + sessions
│   ├── stats.js          ← statistiques + heatmap
│   ├── goals.js          ← objectifs + export/import
│   └── main.js           ← point d'entrée
├── nginx.conf
├── Dockerfile
└── docker-compose.yml
```

## 🌐 Déploiement

| Service | Commande |
|---|---|
| **Netlify Drop** | Glisse le dossier sur [app.netlify.com/drop](https://app.netlify.com/drop) |
| **GitHub Pages** | Settings → Pages → Source: main |
| **VPS** | `docker compose up -d` |

## 📄 Licence

Projet personnel — tous droits réservés.
