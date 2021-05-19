# Computer architecture TD6

## Exercice 1

D: check what's in the address (`ADD IM R1 100`: check what's at address 100)      
Im: check the value (`ADD IM R1 100`: use 100) 

__20__    
```python
# R1 = 20
ADD Im R1 -10
# R1 = 10
ADD IM R1 100
# R1 = 110
JMPZ ET1
# Jump to ET1 if R1 = 0 
JMPN ET2
# Jump to ET2 if R0 < 0
PUSH Rg1 R1
# Add to Rg1 stack R1 value
# R1 added
STOP 
ET1: STORE D R1 100
# Stock R1 value into address 100
STOP
ET2: STORE D R1 50 
# Stock R1 value into address 50
STOP
```

__-90__    
```python
# R1 = -100
ADD Im R1 -10
# R1 = 0
ADD IM R1 100
# R1 = 0
JMPZ ET1
# Jump to ET1 if R1 = 0 
JMPN ET2
PUSH Rg1 R1
STOP 
ET1: STORE D R1 100
# Stock R1 value into address 100
# Stocked
STOP
ET2: STORE D R1 50 
STOP
```

__-120__    
```python
# R1 = -120
ADD Im R1 -10
# R1 = -130
ADD IM R1 100
# R1 = -30
JMPZ ET1
JMPN ET2
# Jump to ET2 if R0 < 0
PUSH Rg1 R1
STOP 
ET1: STORE D R1 100
STOP
ET2: STORE D R1 50 
# Stock R1 value into address 50
# Stocked
STOP
```

## Exercice 2

compilation = 10 000 loc/s + 2 secondes     
compilé = 20 * loc_d, 100 000 inst./s     
interprété = 200 * loc_d, 100 000 inst./s

### 1.
0,1s de temps de compilation     
+ 2s
+      
20 000 / 100 000 = 0.2     
= 2,3s pour le programme compilé     

200 * 1000 = 200 000 inst.     
Total = 2s 

### 2. 
302s pour le programme compilé     
2000s pour le programme interprété     

### 3.
- Compilé: N/10^4 + 2 + 20N/10^5
- Interprété: 200N/10^5
- N/10^4 + 2 + 20N/10^5 = 200N/10^5
- N/10^4 + 20N/10^5 = -2
- 17N/10^4 = -2
- N =20000/17 ~= 1176

À partir de 1177 lignes de code, il devient intéressant de compiler plutôt que d'interpréter le programme


## Exercice 3

r0 = ((((r1*r2) - r3) / ((r1+r4) + r5)) + r6) + r2     

### 1.
- MUL r0, r1, r2
- SUB r0, r0, r3
- ADD r1, r1, r4
- ADD r1, r1, r5
- DIV r0, r0, r1
- ADD r0, r0, r6
- ADD r0, r0, r2

### 2.
MOVE r0, r1 ; r0 - r1
MUL r0, r2 ; r0 *= r2
- SUB r0, r3
- ADD r1, r4
- ADD r1, r5
- DIV r0, r1
- ADD r0, r6
- ADD r0, r2

## Exercice 4

Ce programme calcule la taille d'une chaîne

```c
int compteur = 0, i = 0;
while(string[i] != "\0"){
    compteur++;
    i++;
}
```    
**ou**     
```c
int compteur = 0;
while(*string != "\0"){
    compteur++;
    string++;
}
```   