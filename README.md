# 🦊 Chicken Mines — Le Coq Francis

**Démineur** aux couleurs de **Le Coq Francis** : les mines sont des **renards** 🦊 cachés
autour du poulailler. Jouable dans le navigateur et lançable comme **Mini App Telegram**.

- 🌐 **En ligne :** https://franclecoq.github.io/ChickenMines
- 🤖 **Telegram :** https://t.me/FrancisLeCoqBot/ChickenMines

---

## 🎮 Le jeu en bref

Chaque case cache soit un **renard**, soit un chiffre : le nombre de renards tapis dans les
**8 cases voisines**. À toi de déduire où ils dorment sans jamais en réveiller un.

- **Tape** une case pour l'ouvrir.
- **Appui long** (ou clic droit, ou le bouton **🚩 Mode drapeau**) pour planter un drapeau.
- **Tape un chiffre déjà ouvert** dont tous les renards sont balisés pour ouvrir d'un coup
  les cases restantes autour (*chording*).
- La **première case ouverte est toujours sûre** — les renards ne sont placés qu'après.

Tous les renards balisés et toutes les cases sûres ouvertes → **poulailler sauvé**.
Un seul renard réveillé → partie terminée.

## 🗺️ Niveaux

12 niveaux répartis en 5 mondes, du poulailler tranquille à la nuit des renards.
**Le niveau 1 est gratuit pour tout le monde ; les niveaux 2 à 12 sont réservés aux
détenteurs de $FRANC** (même règle que Chicken Snake).

| Monde | Niveaux | Grille | Renards |
|-------|---------|:------:|:-------:|
| 🌿 Prairie | 1 – 3 | 8×8 → 8×10 | 8 → 12 |
| 🏚 Poulailler | 4 – 6 | 9×11 → 10×12 | 15 → 21 |
| 🌾 La Ferme | 7 – 8 | 10×13 → 10×14 | 24 → 27 |
| 🌪 Chaos | 9 – 10 | 11×14 → 11×15 | 30 → 34 |
| 👑 Légende | 11 – 12 | 12×16 | 41 → 46 |

## 🏅 Score

À la victoire : `renards × 20` points, plus un **bonus de vitesse** qui peut doubler la mise
si tu termines bien en dessous du temps de référence (8 s par renard). Le **meilleur score de
chaque niveau** est mémorisé, et leur somme forme le **score total**.

## 🎁 Bonus

Débloqués par le score total cumulé, un usage par partie :

| Bonus | Débloqué à | Effet |
|-------|:----------:|-------|
| 🔎 **Flair** | 300 pts | Ouvre une case sûre au hasard |
| 🐔 **Balise** | 700 pts | Plante un drapeau sur un vrai renard |
| 🛡 **Bouclier** | 1200 pts | Le prochain renard ouvert est pardonné (il est balisé au lieu de te faire perdre) |

Le **🚩 Mode drapeau** est toujours disponible : il n'est pas un bonus, juste un confort
pour baliser au doigt sans appui long.

---

## 🌍 Langues

Français 🇫🇷 / Anglais 🇬🇧 — bascule via les drapeaux, préférence mémorisée (partagée avec
les autres jeux Francis).

---

## 🔧 Technique

Un seul fichier `index.html` : aucune dépendance, aucun build. Le plateau est une grille DOM
(pas de canvas), redimensionnée à l'écran pour tenir sans scroll sur mobile.

Les visuels de Francis (`assets/coq_*.png`) sont repris de **Chicken Blast**, et le menu —
CSS, en-tête, bouton wallet, barre de statut, liste de niveaux, modales, toasts — est repris
de **Chicken Snake**. Le **renard** et le **drapeau** n'existaient dans aucun autre jeu :
ce sont des SVG vectoriels dessinés pour ce jeu, intégrés directement dans le code.

Le déblocage holder réutilise le même backend que les autres jeux Francis (`/check-franc` sur
Supabase) et le même écran de connexion wallet — un wallet connecté sur un jeu débloque tous
les autres.

---

## LICENCE
© 2026 [$FRANC by FRANCIS LE COQ]. Tous droits réservés. Ce jeu et son code source sont une création originale dans le cadre du projet $FRANC. Le code est fourni à titre de consultation. Toute reproduction, redistribution, modification ou réutilisation, totale ou partielle, sans autorisation écrite préalable de l'auteur est interdite. $FRANC / Le Coq Francis et leurs visuels sont des marques du projet.


© 2026 [$FRANC by FRANCIS LE COQ]. All rights reserved.
This game and its source code are proprietary works created for the $FRANC project.
The source code is made available for inspection purposes only. No part of this game, its source code, assets, or related materials may be copied, reproduced, distributed, modified, published, or otherwise reused without the prior written consent of the copyright holder.
$FRANC, Francis Le Coq, and all related names, logos, characters, and visual identities are trademarks and intellectual property of the project.

🐓 *Cocorico !*
