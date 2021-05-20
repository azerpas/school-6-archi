# Stratégie mémoire

## Introduction
- **Mémoire**: dispositif capable de conserver et restituer une information	
- **Mot mémoire**: ensemble de bits pouvant être lus ou écrits simultanément

### Types: 
- Semi-conducteur (RAM)
- Magnétique (HDD)
- Optique (CD)

### Performance
- **Temps d'accès**: temps nécessaire lecture/écriture
- **Débit**: quantité d'infos lues/écrites en temps (ex: *Mo/s*)

![memcostprice](https://user-images.githubusercontent.com/19282069/119001385-36bf5180-b98c-11eb-9890-e1e60e2afe92.png)

## Modes d'accès
### Accès aléatoire
Utilisé par cache & mem principale	
- Chaque mot associé à une adresse unique
- Taille adresse dépend de capacité
- Opérations: lecture, écriture
### Accès par le contenu
Utilisé par cache
- Pas d'adresse
- Mapping (clé, valeur)
- Opérations: lecture, écriture, existe, retirer
### Accès séquentiel
Archivage important de données		
- Informations unes après autres
- Agi comme une liste (first to next)
- Opérations: début, lecture, écriture, fin
### Accès direct
Utilisé par disques, CD...	
- Informations en blocs
- Chaque bloc a une adresse
- Opérations: lecture, écriture

## Mémoire principale
### Mémoire RAM
*Random Access Memory*, données **temporaires**	
#### 2 types
- DRAM (dynamique): mémoire principale
	- rafraîchissement périodique
	- simples, peu couteuses
- SRAM (statique): caches
	- rafraîchissement inutile
	- rapide, couteuses
### Mémoire ROM
*Read Only Memory*, données **permanentes**
#### 3 types
- ROM: écriture uniq à fabrication
- PROM: écriture uniq après fabrication
- EPROM: écritures illimitées (suppression UV)
- FLASH: écritures illimitées (suppression électronique)

### Organisation 
![orga](https://user-images.githubusercontent.com/19282069/119004429-dbdb2980-b98e-11eb-8fa4-9c15454a6919.png)

## Mémoire cache
- Intermédiaire
- Rapide
- Petite capacité
- Données récentes

![cache](https://user-images.githubusercontent.com/19282069/119005649-e8ac4d00-b98f-11eb-9581-f69150f7dda3.png)

### Principe
**Accès à une adresse mémoire**
- si le bloc contenant l'adresse est dans le cache: **adresse lue**
- sinon: **copie dans le cache, adresse lue**

Page 177
## Mémoire externe

## Mémoire virtuelle


