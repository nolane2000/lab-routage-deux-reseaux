# Lab réseau - Routage entre deux réseaux

## Objectif
Mettre en place une communication entre deux réseaux différents à l'aide d'un routeur sur Cisco Packet Tracer.

## Topologie
- 2 PC
- 1 switch
- 1 routeur

## Configuration IP

### Réseau 1
- PC1 : 192.168.1.10 /24
- Gateway : 192.168.1.254

### Réseau 2
- PC2 : 192.168.2.10 /24
- Gateway : 192.168.2.254

## Configuration du routeur
- Interface G0/0/0 : 192.168.1.254
- Interface G0/0/1 : 192.168.2.254

## Résultat
Communication réussie entre les deux réseaux.

## Compétences
- configuration IPv4
- routage
- CLI Cisco