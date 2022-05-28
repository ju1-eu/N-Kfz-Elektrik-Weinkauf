# FM Nr. 6 Übungsaufgaben

## Parallelschaltung

Mathebuch S. 82 Aufgabe 4) a, b, c


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
# Aufgabe 4a
# geg:
R_1 = 30 # Ohm
R_2 = 20 # Ohm
U = 12.6 # V
# ges: I_ges, I_1, I_2, R_ges
# Formel:
I_1 = U / R_1
I_2 = U / R_2
I_ges = I_1 + I_2
R_ges = U / I_ges
# Ausgabe: print("U =", round(U, 4), "V")
print("I_1 =", round(I_1, 4), "A")
print("I_2 =", round(I_2, 4), "A")
print("I_ges =", round(I_ges, 4), "A")
print("R_ges =", round(R_ges, 4), "Ohm")
# Lösung:
# 
```

    I_1 = 0.42 A
    I_2 = 0.63 A
    I_ges = 1.05 A
    R_ges = 12.0 Ohm



```python
# Aufgabe 4b
# geg:
I_1 = 0.3 # A
I_2 = 0.2 # A
U = 14.4 # V
# ges: I_ges, R_ges, R_1, R_2
# Formel:
I_ges = I_1 + I_2
R_ges = U / I_ges
R_1 = U / I_1
R_2 = U / I_2
# Ausgabe: print("U =", round(U, 4), "V")
print("I_ges =", round(I_ges, 4), "A")
print("R_ges =", round(R_ges, 4), "Ohm")
print("R_1 =", round(R_1, 4), "Ohm")
print("R_2 =", round(R_2, 4), "Ohm")
# Lösung:
# 
```

    I_ges = 0.5 A
    R_ges = 28.8 Ohm
    R_1 = 48.0 Ohm
    R_2 = 72.0 Ohm



```python
# Aufgabe 4c
# geg:
I_ges = 1.2 # A
I_2 = 0.3 # A
R_ges = 187.5 # Ohm
# ges: I_1, R_1, R_2, U
# Formel:
# I_ges = I_1 + I_2
I_1 = I_ges - I_2
U = R_ges * I_ges
R_1 = U / I_1
R_2 = U / I_2
# Ausgabe: print("U =", round(U, 4), "V")
print("I_1 =", round(I_1, 4), "A")
print("U =", round(U, 4), "V")
print("R_1 =", round(R_1, 4), "Ohm")
print("R_2 =", round(R_2, 4), "Ohm")
# Lösung:
# 
```

    I_1 = 0.9 A
    U = 225.0 V
    R_1 = 250.0 Ohm
    R_2 = 750.0 Ohm



```python

```
