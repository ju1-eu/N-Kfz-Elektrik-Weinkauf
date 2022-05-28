# FM Nr. 3 Übungsaufgaben

## Reihenschaltung


```python
import math as ma
import numpy as np
# round(Zahl, Stellen))# 4 Stellen nach Komma runden
# print("l = ", round(l, 4), "m")
# Potenz: 2**3 = 2^3
# Wissenschaftliche Schreibweise
#zahl_1 = float(0.0003648) # Ohm = 0.3648 mOhm = 0.0003648 Ohm = 3.648e-04 Ohm
#print(np.format_float_scientific(zahl_1, precision = 4, exp_digits=2))
#zahl_2 = float(2.6667e-03) # Ohm = 2.666666 mOhm = 0.002666666 Ohm = 2.6667e-03 Ohm
#print(np.format_float_scientific(zahl_2, precision = 4, exp_digits=2))
# Schleife: von 1 bis 10 
#for i in range (1,11,1):
#    print(i*i)
# Terminal: jupyter notebook
```


```python
# Aufgabe 1
# geg:
R_1 = 40 # Ohm
R_2 = 110 # Ohm
R_3 = 50 # Ohm
U_2 = 4.4 # V
# ges: U_1, U_3
# Lösung:
I = U_2/R_2
U_1 = R_1 * I
U_3 = R_3 * I
#print("U = ", round(U, 4), "V")
print("I = ", round(I, 4), "A")
print("U_1 = ", round(U_1, 4), "V")
print("U_3 = ", round(U_3, 4), "V")
# I =  0.04 A
# U_1 =  1.6 V
# U_3 =  2.0 V
```


```python
# Aufgabe 2
# geg:
R_1 = 8 # Ohm
R_2 = 24 # Ohm
U_ges = 12 # V
I = 0.27 # A = 270 mA
# ges: R_3, U_1, U_2, U_3
# Lösung:
R_ges = U_ges/I
# R_ges = R_1 + R_2 + R_3
R_3 = R_ges - R_1 - R_2
U_1 = R_1 * I
U_2 = R_2 * I
U_3 = R_3 * I
#print("U = ", round(U, 4), "V")
print("R_ges = ", round(R_ges, 4), "Ohm")
print("R_3 = ", round(R_3, 4), "Ohm")
print("U_1 = ", round(U_1, 4), "V")
print("U_2 = ", round(U_2, 4), "V")
print("U_3 = ", round(U_3, 4), "V")
# R_ges =  44.4444 Ohm
# R_3 =  12.4444 Ohm
# U_1 =  2.16 V
# U_2 =  6.48 V
# U_3 =  3.36 V
```


```python
# Aufgabe 3
# geg: 
R_1 = 22 # Ohm
R_2 = 22 # Ohm
R_3 = 22 # Ohm
I_1 = 0.87 # A = 870 mA
I_delta = 0.075 # A = 75 mA
# ges: R_4, U_1, U_2, U_3, U_4
# Lösung:
I_2 = I_1 - I_delta
R_ges1 = R_1 + R_2 + R_3
U_ges = R_ges1 * I_1
R_ges2 = U_ges/I_2
# R_ges = R_1 + R_2 + R_3 + R_4
R_4 = R_ges2 - R_1 - R_2 - R_3
U_4 = R_4 * I_2
U_1 = R_1 * I_2
#print("U = ", round(U, 4), "V")
print("I_2 = ", round(I_2, 4), "A")
print("R_ges1 = ", round(R_ges1, 4), "Ohm")
print("U_ges = ", round(U_ges, 4), "V")
print("R_ges2 = ", round(R_ges2, 4), "Ohm")
print("R_4 = ", round(R_4, 4), "Ohm")
print("U_4 = ", round(U_4, 4), "V")
print("U_1 = ", round(U_1, 4), "V")
# I_2 =  0.795 A
# R_ges1 =  66 Ohm
# U_ges =  57.42 V
# R_ges2 =  72.2264 Ohm
# R_4 =  6.2264 Ohm
# U_4 =  4.95 V
# U_1 =  17.49 V
# R_1 = R_2 = R_3 => U_1 = U_2 = U_3
```


```python
# Aufgabe 4
# geg:
U_ges = 12 # V
I_1 = 1.75 # A 
U_La = 8.6 # V
# ges: R_ü, I_tat
# Lösung:
# U_ges = U_La + U_Rü
U_Rü = U_ges - U_La
R_La = U_ges/I_1
I_tat = U_La/R_La
R_ü = U_Rü/I_tat
#print("U = ", round(U, 4), "V")
print("U_Rü = ", round(U_Rü, 4), "V")
print("R_La = ", round(R_La, 4), "Ohm")
print("I_tat = ", round(I_tat, 4), "A")
print("R_ü = ", round(R_ü, 4), "Ohm")
# U_Rü =  3.4 V
# R_La =  6.8571 Ohm
# I_tat =  1.2542 A
# R_ü =  2.711 Ohm
```


```python

```
