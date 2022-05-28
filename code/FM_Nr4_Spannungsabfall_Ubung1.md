# FM Nr. 4 Übungsaufgaben

## Spannungsabfall

Tabellenbuch S. 280 Nennquerschnitt


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
A = 0.6 # mm^2
p = 0.3 # Ohm x mm^2/m
I = 8 # A
U_v = 4 # V
# ges: l
# Formel:
# U_v = p * l * I/A =>
l = (U_v * A)/(p * I)
# Ausgabe: print("U =", round(U, 4), "V")
print("l =", round(l, 4), "m")
# Lösung:
# l = 1.0 m
```

    l = 1.0 m



```python
# Aufgabe 2
# geg:
l = 4 # m (Kupfer)
U_ges = 10 # V
U_k = 9.6 # V
I = 150 # A
p = 0.0178 # Ohm x mm^2/m
# ges: A_mind, R_st, A
# Formel:
R_st = U_k/I
# U_v = U_ges - U_k => A_mind = p * l * I/U_v =>
A_mind = p * l * I/(U_ges - U_k)
# Ausgabe: print("U =", round(U, 4), "V")
print("R_st =", round(R_st, 4), "Ohm")
print("A_mind =", round(A_mind, 4), "mm^2")
# Lösung:
# R_st = 0.064 Ohm
# A_mind = 26.7 mm^2 => A_Nenn = 35 mm^2 (Nennquerschnitt)
```

    R_st = 0.064 Ohm
    A_mind = 26.7 mm^2



```python
# Aufgabe 3
# geg:
A = 0.75 # mm^2
l = 6 # m (Kupfer)
U_v = 0.3 # V = 300 mV
p = 0.0178 # Ohm x mm^2/m
# ges: I
# Formel:
# U_v = p * l * I/A =>
I = U_v * A/(p * l)
# Ausgabe: print("U =", round(U, 4), "V")
print("I =", round(I, 4), "A")
# Lösung:
# I = 2.1067 A
```

    I = 2.1067 A



```python
# Aufgabe 4
# geg:
l = 4.5 # m (Kupfer)
l_1 = 2.25 # m (Plusleitung)
l_2 = 2.25 # m (Minusleitung)
U_v = 0.3 # V
U_B = 12.4 # V
p = 0.0178 # Ohm x mm^2/m
I = 156 # A
# ges: A_mind, A_Nenn, R_st
# Formel:
# U_k = U_B - U_v1 - U_v2 => R_st = U_k/I =>
R_st = (U_B - U_v - U_v)/I
# U_v = p * l * I/A =>
A_mind = p * l_1 * I/U_v
# Ausgabe: print("U =", round(U, 4), "V")
print("R_st =", round(R_st, 4), "Ohm")
print("A_mind =", round(A_mind, 4), "mm^2")
# Lösung:
# R_st = 0.0756 Ohm
# A_mind = 20.826 mm^2 => A_Nenn = 25 mm^2 (Nennquerschnitt)
```

    R_st = 0.0756 Ohm
    A_mind = 20.826 mm^2



```python
# Aufgabe 5
# geg:
l = 1.65 # m (Kupfer)
U_v_proz = 2.5 # % von 12 V
U_ges = 12 # V 
p = 0.0178 # Ohm x mm^2/m
I = 50 # A
# ges: A_Nenn
# Formel:
# U_v_proz = U_v * 100/U_ges =>
U_v = U_v_proz * U_ges/100
# U_v = p * l * I/A =>
A_mind = p * l * I/U_v
# Ausgabe: print("U =", round(U, 4), "V")
print("U_v =", round(U_v, 4), "V")
print("A_mind =", round(A_mind, 4), "mm^2")
# Lösung:
# U_v = 0.3 V
# A_mind = 4.895 mm^2 => A_Nenn = 6 mm^2 (Nennquerschnitt)
```

    U_v = 0.3 V
    A_mind = 4.895 mm^2



```python
# Aufgabe 6
# geg:
U_v = 0.10385232 # V = 103.85232 mV
p = 0.0178 # Ohm x mm^2/m
I = 1.87 # A
A = 1.5 # mm^2
# ges: 
# Formel:
# U_v = p * l * I/A =>
l = (U_v * A)/(p * I)
# Ausgabe: print("U =", round(U, 4), "V")
print("l =", round(l, 4), "m")
# Lösung:
# l = 4.68 m
```

    l = 4.68 m



```python

```
