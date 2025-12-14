# TP 2 : Dashboard météo en temps réel avec WebSocket (Node.js + CSV + Chart.js)

---
##  Format du fichier CSV (`temp.csv`)

Exemple :

```
mois,tmax,tmin,pluie
Jan,18,8,6
Fev,20,9,4
Mar,23,11,4
```

Chaque ligne représente les données météo d’un mois.

---

##  Fonctionnement du serveur (`app2.js`)

Le serveur WebSocket :
1. Écoute sur le port **5002**
2. Lit le fichier `temp.csv`
3. Convertit le CSV en JSON
4. Envoie **une ligne toutes les 3 secondes** à chaque client connecté

### Lancement du serveur

```bash
node app2.js
```

Message attendu :
```
Serveur WebSocket actif : ws://localhost:5002
Client connecté
```
<img width="464" height="221" alt="Screenshot 2025-12-14 150708" src="https://github.com/user-attachments/assets/3de54c1c-bdc0-4b94-8b67-7c42acb1e449" />

---

##  Fonctionnement côté client

- Le navigateur se connecte au serveur WebSocket
- Il reçoit les données météo au format JSON
- Les graphiques Chart.js sont mis à jour dynamiquement
- Les données apparaissent progressivement (effet temps réel)

---

##  Résultat attendu

- Connexion WebSocket fonctionnelle
- Réception des données toutes les 3 secondes
- Graphiques météo mis à jour en temps réel
- Aucune erreur dans la console

<img width="959" height="506" alt="Screenshot 2025-12-14 150154" src="https://github.com/user-attachments/assets/8a84f79e-fb1e-4791-8b89-cb8ca494d72c" />


---



##  Étudiant : Hadil Zaimi

##  Cours : **Développement web full-stack avec JavaScript**

---


