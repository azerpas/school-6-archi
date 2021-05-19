# Computer Architecture TD7

## Exercice 1

- Little endian
- Big endian    
Ici on groupe par paquet de 2 ou 4 octets    

a. 123A0010 D644944E     
Pas illégaux, dans l'ordre, donc big endian
b. 123A001A 2D87      
2 octets, pas illégaux, dans le désordre donc little endian     
c. 123A0031 D680 A8D1    
pas allignés, illégal, moyen de trouver (123A0031) impair donc illégal
d. 123A0020 EE480D3A403F65A8        
little endian, on commence de la fin       
e. 123A002C 1B896F47     
alligné, big endian
f. 123A002B 9B1B896F     
illégal, non aligné, B impair 
g. 123A001E 5B59
big endian
h. 123A0009 30
alligné, à la fois du little et du big     
i. 123A000B BDD9
pas alligné donc illégal

## Exercice 5
- Interruption externe provenant d’un périphérique
- Tentative d’exécution d’une instruction illégale
- Interruption thermique indiquant une surchauffe du processeur
- Appel système (SYSCALL) 


1. Instruction illégale     
Pas le droit donc on le bloque direct
2. Appel système     
Processus en attente, embêtant. On le débloque le plus rapidement   
3. Interruption externe provenant d'un périphérique
4. Interruption thermique indiquant une surchauffe du processeur


## Exercice 3
