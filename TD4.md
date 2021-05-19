# Computer architecture TD4

## Exercice 1

### 1.

Composé de 16 bits = 2 octets     

- 77(8)
- 100(8)
- 101(8)
- 102(8)
...
- 107(8)
- 110(8)
- 111(8)
- 112(8)

5 élément car on part du premier     
Or on a 2 octets donc 2\*5 = 10      
10(10) = 12(8)     
77(8) + 12(8) = 111(8) 

### 2.

77(8) = 63

### 3.
8 b -> 2 Mi     
16 b -> 1 Mi      
32 b -> 512 Ki      

## Exercice 2

32 bits     

### 1.
2^32 = 4Gib mots    
### 2.
2^32 - 1
### 3.
Taille d'un mot ne change rien au nombre de mots adressables      
Ça multiplie par contre la taille de la mémoire par 4     
Donc tonjours 2^32
### 4.
2^32 - 1

## Exercice 3

32 octets / 50 ns = 32 octets / 50 s \* 10^-9     
640 mo / s 

## Exercice 4

### 1.
2^16 mots     
2^16 \* 32 bits = 2048 kib = 2 Mib     

### 2.
16 bits - taille index - taille offset =   
taille offset: (4\*4) = 16 octets = 2^4 = 4 bits     
taille index: 4 lignes, 2 bits      
16 bits - 4 - 2 = 10 bits     

### 3.

4 lignes * (10 bits) * 1 bit * (32\*4) = 4\*139 = 556     

lignes * tags * ctrl * mots\*taille mot