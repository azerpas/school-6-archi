# Représentation de l'information

## Bases
![bases](https://user-images.githubusercontent.com/19282069/118866099-f60afe00-b8e1-11eb-866f-1f76066e968e.png)

### Base 2
{0,1}	
01101(2) = 0*2^4 + 1*2^3 + 1*2^2 + 0*2^1 + 1*2^0 = 8(10) + 4(10) + 1(10) = 13(10)

### Base 16
{0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F}	
01B(16) = 0*16^2 + 1*16^1 + 11*16^0 = 16(10) + 11(10) = 27(10)

## Autres représentations

- Code ASCII (7 bits + 1 bit de parité)
- Unicode

## Conversion base 10 vers base B
### Division avec reste
100(10) -> base 8	  
```
100÷8: quotient 12, reste 4	
12÷8: quotient 1, reste 4	
1÷8: quotient 0, reste 1
```
**100(10) = 144(8)**

## Représentations des nombres négatifs
### Signe et valeur absolue 
**Signe**: poids fort		
#### Exemple sur 3 bits [-3,3]
000: 0	  
001: 1    	    
010: 2	      
011: 3	  
100: 0	  
101: -1		  
110: -2		  
111: -3		  

### Complément à 2
Complément à 1 + 1
#### Exemple sur 3 bits [-4,3]
000: 0
001: 1
010: 2
011: 3
100: -4
101: -3
110: -2
111: -1

## Circuits combinatoires & séquentiels
- `Algèbre de Boole`: circuits combinatoires
- `Théorie des automates`: circuits séquentiels
- `Signaux logiques et analogiques`

## Table de vérité 
Description d'une opération logique:
![tableverite](https://user-images.githubusercontent.com/19282069/118999906-f14e5480-b98a-11eb-81dc-cda2e19454a2.png)
