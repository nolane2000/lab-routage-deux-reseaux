# 🌐 Lab réseau - Routage entre deux réseaux

## 🎯 Objectif
Mettre en place une communication entre deux réseaux différents à l'aide d'un routeur dans Cisco Packet Tracer.

---

## 🧱 Topologie réseau

- 2 PC (clients)
- 1 switch
- 1 routeur

![Topologie](topologie-routage-deux-reseaux.png)

---

## 🌐 Configuration IP

### Réseau 1
- PC-Client-1 : 192.168.1.10 /24
- Passerelle : 192.168.1.254

### Réseau 2
- PC-Client-2 : 192.168.2.10 /24
- Passerelle : 192.168.2.254

---

## ⚙️ Configuration du routeur (CLI)

enable
configure terminal

interface gigabitethernet 0/0/0
ip address 192.168.1.254 255.255.255.0
no shutdown
exit

interface gigabitethernet 0/0/1
ip address 192.168.2.254 255.255.255.0
no shutdown
exit

end

#Les interfaces du routeur ont été configurées pour permettre la communication entre les deux réseaux.

## Test de connectivité
![Ping réussi](test-ping-reussi.png)

## Résultat
La communication entre les deux réseaux est fonctionnelle.

## Compétences développées
- configuration d'adresses IPv4
- compréhension du routage entre réseaux
- Utilisation du CLI Cisco
- Configuration d'un routeur
- Diagnostic et résolution d'erreurs réseau

## 📁 Fichiers

- lab-routage-deux-reseaux.pkt
- topologie-routage-deux-reseaux.png
- test-ping-reussi.png