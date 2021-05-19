# TD1

## 1.Calculer le temps (en termes de top d’horloge) nécessaire pour l’exécution de l’opération suivante : `X = Y + Z`

7 operations:     
1. Put the Y in the Address Register (AR)
2. Retrieve Y with the Information Register (IR) and pass it to the Arithmetic and Logical Unit (ALU)
3. Put the Z in the Address Register (AR)
4. Retrieve Z with the Information Register (IR) and pass it to the Arithmetic and Logical Unit (ALU)
5. Execute Y + Z and deposit the result into the Accumulator (ACC), an intermediate storage register that lays inside the CPU
6. Put the result (X) inside the Address Register (AR)
7. Transfer X from the AR to the main memory address stocked inside the AR address registery

## 2. Memory of a computer

### 1) Determine the size of the memory words and the capacity of this box in
KB.

As we can on the memory, it carries 12 entries that encode the addresses of a mememory word.          
We just need to pass it to bytes: 2^12 * 8 bits = 2^10 bytes * 2^2 bytes * 1 byte = 4096 bytes = 4 KB 

### 2) By assembling boxes of this type: how to create a 4K word 16-bit memory
space?

[TD1_1](TD1_1.png)
