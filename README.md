# 💰 Budget Foyer — Application Mobile v3

Application web progressive (PWA) complète de gestion budgétaire pour un foyer.
**Installable sur iPhone et Android comme une vraie app, sans App Store.**

---

## 📱 5 onglets

| Onglet | Contenu |
|--------|---------|
| 📊 **Tableau de bord** | KPIs, progression budget, courbes multi-graphiques, comparatif Budget/Réel, trésorerie cumulée |
| 💰 **Revenus** | CDI, Entreprise Individuelle (EI), Primes, Dividendes, Rentes — par conjoint + prorata |
| 📋 **Budget** | Postes renommables, montants modifiables, récurrence (tous les mois / personnalisé / ponctuel) |
| 🐖 **Cagnottes** | Épargne progressive pour dépenses annuelles — graphique de cumul + impact trésorerie |
| ✏️ **Réel** | Saisie mensuelle des dépenses réelles + comparatif automatique Budget/Réel |

---

## 🚀 Déploiement GitHub Pages (5 min)

### 1. Créer un dépôt GitHub
1. Connectez-vous sur [github.com](https://github.com)
2. **New repository** → nom : `budget-foyer` → **Public** → **Create**

### 2. Uploader les fichiers
1. Dans le dépôt → **Add file › Upload files**
2. Glissez-déposez les 5 fichiers :
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
3. **Commit changes**

### 3. Activer GitHub Pages
1. **Settings** › **Pages**
2. Source : **Deploy from a branch**
3. Branch : **main** · Folder : **/ (root)**
4. **Save**

⏳ 1-2 minutes d'attente, puis l'app est disponible à :
```
https://VOTRE_PSEUDO.github.io/budget-foyer/
```

---

## 📲 Installer sur téléphone

### iPhone (Safari uniquement)
1. Ouvrez l'URL dans **Safari** (pas Chrome, pas Firefox)
2. Icône **Partager** (carré avec flèche ↑)
3. **"Sur l'écran d'accueil"**
4. **Ajouter**

### Android (Chrome)
1. Ouvrez l'URL dans **Chrome**
2. Menu **⋮** → **"Ajouter à l'écran d'accueil"**
3. **Ajouter**

L'app s'installe avec son icône, fonctionne **hors-ligne** et s'ouvre en plein écran.

---

## 🔒 Confidentialité totale

Toutes les données sont stockées **uniquement sur votre appareil** (localStorage du navigateur).
Aucun serveur, aucun compte, aucune donnée transmise.

---

## ✨ Fonctionnalités détaillées

### Revenus
- **CDI** : salaire principal net
- **EI** : revenu d'entreprise individuelle (séparé, badge dédié)
- **Prime** : revenus exceptionnels variables par mois
- **Dividendes** et **rentes locatives**
- Calcul automatique du prorata de contribution de chaque conjoint

### Budget
- Renommez chaque poste directement dans l'app
- Récurrence **tous les mois**, **personnalisée** (cochez les mois) ou **ponctuelle**
- Ajout et suppression de postes à la volée

### Cagnottes
- Définissez un **nom**, un **objectif annuel**, un **montant mensuel** et un **mois d'échéance**
- La courbe repart de zéro après le mois d'échéance
- Graphique de **cumul mois par mois** — une courbe par cagnotte
- Graphique de **trésorerie disponible** : avec vs. sans cagnottes

### Comptes Réels
- Saisie mois par mois, poste par poste
- Écart Budget/Réel affiché en temps réel (vert = économie, rouge = dépassement)
- Barre de progression par catégorie dans le tableau de bord

---

## 🛠 Personnalisation avancée

Pour modifier les postes par défaut ou les cagnottes pré-remplies, éditez les tableaux
`DEFAULT_EXPENSES` et `DEFAULT_CAGNOTTES` dans `index.html` (vers la ligne 200).

---

*Budget Foyer v3 · 2024*
