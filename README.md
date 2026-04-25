# Site Ghizlane Daghouj

Site CV one-page pour **Ghizlane Daghouj** — agente administrative & commerciale trilingue, basée à Belvaux (Luxembourg).

## Aperçu

- **Une seule page HTML** autonome (pas de framework, pas de build).
- **Palette éditoriale** crème rosé `#f7f1ea` + bordeaux `#8a3a3a` + champagne `#c89a7c`.
- **Typographies** Inter (corps) + Instrument Serif italique (accents éditoriaux) + Caveat (signature manuscrite) + Amiri (calligraphie arabe).
- **Mode clair / sombre** persisté en localStorage.
- **Mode "recruteur pressé"** — toggle dans la nav qui condense la page pour une lecture rapide.
- **Bouton "Imprimer en PDF"** avec feuille de style print A4 dédiée.
- **Effets** : compteurs animés au scroll, barre de progression de lecture, curseur custom, mini-table des matières flottante, pilule glissante dans la nav, signature manuscrite avant le footer.

## Structure

```
Site Ghizlane/
├── index.html                  # Toute la page (HTML + CSS + JS inline)
├── photo.jpg                   # Portrait monochrome chaud (4:5)
├── photo.png                   # Variante PNG du portrait
├── CV_Ghizlane_Daghouj.pdf     # CV téléchargeable depuis le site
└── README.md
```

## Sections du site

1. **Hero** — Nom, titre XXL, photo, 3 chiffres-clés animés (8 ans, 120+ dossiers, 3 langues), CTA Contacter / Télécharger CV / LinkedIn.
2. **Marquee** — Bandeau défilant des compétences clés.
3. **Profil** — Lead éditorial avec lettrine + carte de visite latérale.
4. **Expérience** — 4 postes (ALD Automotive, A&A Gérance, S.Oliver / Comma, Cactus) avec storytelling et chiffres-clés.
5. **Carrière en chiffres** — Mini-dashboard 6 tuiles (8 ans, 4 entreprises, 960+ dossiers, 50k e-mails, 3 langues, 2080 jours).
6. **Compétences** — Bento grid (compétences clés, langues, Pack Office, soft skills).
7. **Parcours** — Formation + centres d'intérêt.
8. **Côté humain** — Trois adjectifs (Rigoureuse · Calme · Fiable).
9. **Salutation arabe** — السَّلامُ عَلَيْكُمْ en pleine largeur.
10. **Contact** — Bloc bordeaux avec CTAs (e-mail, CV, LinkedIn, imprimer) + carte d'infos pratiques.
11. **Signature** — *« Au plaisir d'échanger, »* + signature manuscrite *Ghizlane*.

## Workflow Git

- `main` → branche stable (le site déployé en production).
- `dev` → branche de travail (modifs + tests avant merge).

Pour modifier le site :

```bash
git checkout dev
# faire les changements
git add .
git commit -m "description du changement"
git push origin dev
```

Quand la version est validée, ouvrir une **Pull Request** `dev → main` sur GitHub.

## Déploiement

Le site est statique (HTML/CSS/JS pur) — il peut être hébergé n'importe où :
GitHub Pages, Cloudflare Pages, Vercel, Netlify, ou un simple serveur web.

Pour brancher un nom de domaine personnalisé :
- **GitHub Pages** → ajouter un fichier `CNAME` à la racine contenant le domaine, puis configurer les DNS chez le registrar.
- **Cloudflare Pages** → connecter le repo, ajouter le domaine dans l'onglet *Custom domains* du projet.

## Crédits

Design original conçu via Claude Design (claude.ai/design), implémenté avec Claude Code.
