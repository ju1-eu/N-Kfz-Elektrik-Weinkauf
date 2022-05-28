# FM Nr. 3 Übungsaufgaben

## Reihenschaltung

Mathebuch S.82


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
R_1 = 125 # Ohm
R_2 = 250 # Ohm
U = 225 # V
# ges: R_ges, I, U_1, U_2
# Lösung:
R_ges = R_1 + R_2
I = U/R_ges
U_1 = R_1 * I
U_2 = R_2 * I
#print("U = ", round(U, 4), "V")
print("R_ges = ", round(R_ges, 4), "Ohm")
print("I = ", round(I, 4), "A")
print("U_1 = ", round(U_1, 4), "V")
print("U_2 = ", round(U_2, 4), "V")
# R_ges =  375 Ohm
# I =  0.6 A
# U_1 =  75.0 V
# U_2 =  150.0 V
```


```python
# Aufgabe 2
# geg:
U_ges = 235 # V
R_1 = 176 # Ohm
I = 0.25 # A
# ges: U_1, U_2, R_2
# Lösung:
U_1 = R_1 * I
#U_ges = U_1 + U_2
U_2 = U_ges - U_1
R_2 = U_2/I
#print("U = ", round(U, 4), "V")
print("U_1 = ", round(U_1, 4), "V")
print("U_2 = ", round(U_2, 4), "V")
print("R_2 = ", round(R_2, 4), "Ohm")
# U_1 =  44.0 V
# U_2 =  191.0 V
# R_2 =  764.0 Ohm
```


```python

```
