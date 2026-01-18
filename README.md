# Quiz Secouriste Suisse 🇨🇭

Quiz interactif pour tester les connaissances des secouristes selon les standards suisses.

![Quiz Secouriste](https://img.shields.io/badge/version-1.0.0-E30613)
![License](https://img.shields.io/badge/license-MIT-blue)
![Swiss Standards](https://img.shields.io/badge/conforme-SRC%20%7C%20IAS%20%7C%20SSS-green)

## 🎯 Objectif

Cet outil de formation permet aux secouristes suisses de tester et renforcer leurs connaissances à travers 90 questions réparties en 3 niveaux de difficulté.

## 📚 Niveaux

| Niveau | Nom | Public cible | Contenu |
|--------|-----|--------------|---------|
| 1 | **BLS-AED** | Grand public, First Responders | Réanimation, DAE, positions d'attente |
| 2 | **Secouriste** | Samaritains, secouristes d'entreprise | ABCDE, traumatismes, urgences médicales |
| 3 | **Médecine de catastrophe** | Secouristes avancés | Triage START/SALT, afflux massif, coordination |

## ✨ Fonctionnalités

- ✅ 90 questions basées sur les directives suisses officielles
- ✅ Mix de QCM simple et choix multiples
- ✅ Correction immédiate avec explications
- ✅ Références aux sources (SRC, IAS, SSS)
- ✅ Design responsive (mobile/desktop)
- ✅ Accès libre aux 3 niveaux
- ✅ Seuil de réussite à 80%
- ✅ Hébergeable sur GitHub Pages (100% statique)

## 🚀 Déploiement sur GitHub Pages

### Option 1 : Déploiement direct

1. Créez un nouveau repository sur GitHub
2. Uploadez tous les fichiers du dossier `quiz-secouriste-ch`
3. Allez dans **Settings** → **Pages**
4. Sélectionnez la branche `main` et le dossier `/ (root)`
5. Cliquez sur **Save**

Votre quiz sera accessible à : `https://votre-username.github.io/nom-du-repo/`

### Option 2 : Via Git

```bash
# Clonez ou initialisez votre repo
git clone https://github.com/votre-username/quiz-secouriste.git
cd quiz-secouriste

# Copiez les fichiers du projet
# ...

# Poussez vers GitHub
git add .
git commit -m "Initial commit - Quiz Secouriste Suisse"
git push origin main
```

## 📁 Structure du projet

```
quiz-secouriste-ch/
├── index.html              # Page d'accueil
├── quiz.html               # Interface du quiz
├── results.html            # Page des résultats
├── README.md               # Documentation
├── css/
│   └── style.css           # Styles responsive
└── js/
    ├── quiz-engine.js      # Moteur du quiz
    └── questions/
        ├── niveau1.js      # 30 questions BLS-AED
        ├── niveau2.js      # 30 questions Secouriste
        └── niveau3.js      # 30 questions Catastrophe
```

## 📝 Personnalisation des questions

Les questions sont stockées dans les fichiers `js/questions/niveauX.js`. Chaque question suit ce format :

```javascript
{
    question: "Texte de la question ?",
    type: "single",  // ou "multiple" pour choix multiples
    answers: [
        { text: "Réponse A", correct: false },
        { text: "Réponse B", correct: true },
        { text: "Réponse C", correct: false },
        { text: "Réponse D", correct: false }
    ],
    explanation: "Explication pédagogique...",
    source: "SRC Guidelines 2021"
}
```

### Types de questions

- `single` : Une seule bonne réponse (boutons radio)
- `multiple` : Plusieurs bonnes réponses possibles (cases à cocher)

## 📖 Sources de référence

- **[Swiss Resuscitation Council (SRC)](https://www.resuscitation.ch)** - Guidelines BLS/AED
- **[Interassociation de Sauvetage (IAS)](https://www.ivr-ias.ch)** - Directives secourisme
- **[Fédération Suisse des Samaritains (SSS)](https://www.samariter.ch)** - Formation secouriste
- **Plan ORCA** - Organisation des secours en cas de catastrophe

## ⚖️ Licence

MIT License - Libre d'utilisation et de modification.

## ⚠️ Avertissement

Cet outil est destiné à la **formation et à l'entraînement** uniquement. Il ne remplace pas une formation officielle certifiée. En cas de doute sur une procédure, référez-vous toujours aux directives officielles et à votre formateur.

---

Développé avec ❤️ pour la communauté des secouristes suisses
