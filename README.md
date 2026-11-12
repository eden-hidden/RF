# RF
Analyseur de spectre RF -EDEN JOHEIR


<img width="770" height="434" alt="Capture d’écran 2026-11-12 à 22 21 06" src="https://github.com/user-attachments/assets/9af3a0d3-5e49-4820-a853-87229a70c092" />






## 1. Définition et principe de base

Un **analyseur de spectre RF** (Radiofréquence) est un instrument de mesure électronique utilisé pour observer la répartition de l'énergie d'un signal en fonction de sa fréquence.

Contrairement à un oscilloscope (qui affiche l'évolution d'un signal dans le **temps**) ou à un VNA (qui émet son propre signal), l'analyseur de spectre est un appareil **passif** : il « écoute » les signaux entrants (via un câble ou une antenne) et les décompose en leurs différentes composantes fréquentielles (grâce à la transformée de Fourier rapide, FFT, ou par balayage hétérodyne).

---

## 2. Que mesure-t-on exactement ?

L'analyseur de spectre permet de caractériser les signaux radioélectriques présents dans un environnement ou issus d'un émetteur :

* **La puissance du signal (en dBm) :** Mesure l'amplitude (la force) de chaque fréquence détectée.
* **La fréquence centrale et la largeur de bande :** Permet d'identifier précisément sur quelle fréquence un émetteur travaille (ex. : $2,4\text{ GHz}$ pour le Wi-Fi) et quelle largeur de canal il occupe.
* **Les signaux parasites et harmoniques :** Détecte les interférences, les fuites électromagnétiques ou les distorsions générées par un composant électronique (comme un amplificateur qui sature).
* **Le rapport signal sur bruit (SNR) :** Évalue la qualité d'une liaison en comparant la puissance du signal utile au niveau du bruit de fond.

---

## 3. L'affichage : le domaine fréquentiel

Sur l'écran d'un analyseur de spectre, le graphique est toujours structuré de la même manière :

* **Axe horizontal (abscisse) :** La **fréquence** (en $\text{Hz}$, $\text{kHz}$, $\text{MHz}$ ou $\text{GHz}$), de la plus basse à gauche à la plus haute à droite.
* **Axe vertical (ordonnée) :** L'**amplitude** ou la **puissance** du signal (généralement exprimée sur une échelle logarithmique en $\text{dBm}$).

Chaque signal présent apparaît sous la forme d'un **pic** vertical. Plus le pic est haut, plus le signal est puissant à cette fréquence précise.

---

## 4. Les réglages essentiels pour une bonne mesure

Pour obtenir une lecture fiable sans endommager l'appareil, trois paramètres principaux doivent être configurés :

1. **Center Frequency & Span :** Définit la fréquence centrale observée et la largeur de la fenêtre d'analyse autour de ce point (le *Span*).
2. **RBW (Resolution Bandwidth) :** Règle la finesse du filtre d'analyse. Un RBW faible permet de séparer deux signaux très proches et de réduire le bruit de fond, mais ralentit le balayage de l'écran.
3. **Reference Level & Atténuation :** Ajuste l'échelle verticale et protège l'entrée de l'appareil contre les signaux trop puissants qui risqueraient de saturer ou de griller le récepteur.
