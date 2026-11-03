# Arduino - Thérémine Lumineux

Un projet permettant de créer un instrument de musique (type thérémine) dont la hauteur de la note varie en fonction de la lumière captée par une photorésistance.

## 📸 Schéma du montage physique

![Montage du Thérémine Lumineux](TheremineLumineux/TheremineLumineux.JPG)

## 🛠️ Composants utilisés
- 1x Carte **Arduino Uno**
- 1x **Photorésistance (LDR)** associée à une résistance de **10 kΩ** (pont diviseur de tension)
- 1x **Buzzer** (relié à la broche numérique `8`)
- 1x **Breadboard** et des fils de connexions

## 🧠 Principe de fonctionnement
1. **Capteur :** La photorésistance fait varier la tension électrique transmise à la broche analogique `A0` selon l'intensité lumineuse perçue.
2. **Calibrage :** Au démarrage, une boucle enregistre automatiquement les seuils minimums et maximums de lumière de la pièce.
3. **Son :** L'Arduino convertit cette valeur lumineuse en une fréquence sonore jouée en temps réel par le buzzer.

## 💻 Code Source
Le code source complet de ce projet se trouve dans le fichier [`TheremineLumineux/TheremineLumineux.ino`](TheremineLumineux/TheremineLumineux.ino).
