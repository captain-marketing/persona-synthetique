# Plugin — Persona Synthétique

**Transforme tes données clients en personas vivants, simulables et évolutifs.**

Créé par [Captain Marketing](https://captainmarketing.io) — Stéphane Truphème

---

## Ce que fait ce plugin

La plupart des personas finissent en PDF dans un dossier. Celui-ci fonctionne différemment : il crée des entités conversationnelles capables d'objecter, d'hésiter, de résister — et de simuler ce qu'un vrai client ferait face à ton pitch, ton offre ou ton argumentaire.

La matière première prioritaire : tes transcriptions AI Notetaker. Pas des suppositions marketing, pas un ICP idéalisé — le verbatim brut de ce que tes clients disent (et ne disent pas) en appel.

---

## Installation

### Option 1 — Upload direct dans Cowork (le plus simple)

1. Télécharge le [zip de la dernière release](https://github.com/captain-marketing/persona-synthetique/releases)
2. Dans Claude Desktop → Cowork → **Customize** → **Plugins** → **+**
3. Sélectionne le zip
4. Tape `/reload-plugins` dans la session

### Option 2 — Via marketplace GitHub (pour rester à jour)

Dans une session Claude Code ou Cowork :

```
/plugin marketplace add captain-marketing/persona-synthetique
/plugin install persona-synthetique@captain-marketing-plugins
```

---

## Les 6 commandes

| Commande | Usage |
|----------|-------|
| `/persona-synthetique:persona-creation` | Créer un persona depuis tes données |
| `/persona-synthetique:persona-validation` | Vérifier sa solidité avant de l'utiliser |
| `/persona-synthetique:persona-discussion` | Simuler une conversation avec lui |
| `/persona-synthetique:persona-panel` | Réunir plusieurs personas simultanément |
| `/persona-synthetique:persona-optimisation` | Affiner ce qui sonne faux |
| `/persona-synthetique:persona-context` | Intégrer de nouvelles données terrain |

Tu peux aussi décrire ce que tu veux faire en langage naturel — Claude reconnaît automatiquement quel skill déclencher.

---

## Workflow recommandé

```
/persona-creation  →  colle tes transcriptions
        ↓
/persona-validation  →  challenge le persona
        ↓
/persona-discussion  →  simule une conversation
        ↓
/persona-optimisation  →  affine si besoin
```

---

## Structure du repo

```
persona-synthetique/
├── .claude-plugin/
│   ├── plugin.json          ← manifest du plugin
│   └── marketplace.json     ← manifest de la marketplace
├── skills/
│   ├── persona-creation/SKILL.md
│   ├── persona-validation/SKILL.md
│   ├── persona-discussion/SKILL.md
│   ├── persona-panel/SKILL.md
│   ├── persona-optimisation/SKILL.md
│   └── persona-context/SKILL.md
└── README.md
```

---

## Prérequis

- Claude Desktop avec Cowork activé
- Plan Pro, Max, Team ou Enterprise (Skills nécessitent l'exécution de code)

---

## Licence

MIT — libre d'utilisation, d'adaptation et de redistribution.
