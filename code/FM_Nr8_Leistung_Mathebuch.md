# FM Nr. 8 Übungsaufgaben

## Leistung

Mathebuch 
S. 82 Aufgabe 4d) 
S. 84 Aufgabe 4) 
S. 82 Aufgabe 3)


```python
import math as ma
import numpy as np
# round(Zahl, Stellen))# 4 Stellen nach Komma runden
# print("l = ", round(l, 4), "m")
# Potenz: 2**3 = 2^3
# Wissenschaftliche Schreibweise
# Exponentialschreibweise: \num{2,67e-03} => 2.67 x 10^-3
# Pfeil: \curvearrowright  oder \to
# Mathemodus: https://katex.org/docs/supported.html
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
# Mathebuch S. 82 Aufgabe 4d) 
# geg:
I_ges = 0.35 # A
U = 210 # V
R_2 = 1000 # Ohm = 1 k
# ges: I_1, I_2, R_ges, R_1, P_R_1, P_R_2
# Formel:
R_ges = U / I_ges
I_2 = U / R_2
# I_ges = I_1 + I_2
I_1 = I_ges - I_2
R_1 = U / I_1
P_R_1 = U * I_1
P_R_2 = U * I_2
# Ausgabe: print("U =", round(U, 4), "V")
print("R_ges =", round(R_ges, 4), "Ohm")
print("I_2 =", round(I_2, 4), "A")
print("I_1 =", round(I_1, 4), "A")
print("R_1 =", round(R_1, 4), "Ohm")
print("P_R_1 =", round(P_R_1, 4), "W")
print("P_R_2 =", round(P_R_2, 4), "W")
# Lösung:
# 
```

    R_ges = 600.0 Ohm
    I_2 = 0.21 A
    I_1 = 0.14 A
    R_1 = 1500.0 Ohm
    P_R_1 = 29.4 W
    P_R_2 = 44.1 W



```python
# Mathebuch S. 84 Aufgabe 4) 
# geg: Glühkerze
U_k = 10.5 # V
P_k = 100 # W
# ges: I_k, R_k
# Formel:
# P = U * I
I_k = P_k/U_k
R_k_1 = U_k/I_k # (Var. 1)
# P = U * I
# P = U^2/R
R_k_2 = (U_k * U_k)/P_k # (Var. 2)
# Ausgabe: print("U =", round(U, 4), "V")
print("I_k =", round(I_k, 4), "A")
print("R_k_1 =", round(R_k_1, 4), "Ohm")
print("R_k_2 =", round(R_k_2, 4), "Ohm")
# Lösung:
# 
```

    I_k = 9.5238 A
    R_k_1 = 1.1025 Ohm
    R_k_2 = 1.1025 Ohm



```python
# Mathebuch S. 82 Aufgabe 3)
# geg: Leuchtstoffröhre 65V/8W Schaltung
U_ges = 230 # V
U_k_La = 65 # V
l_1 = 5 # m
l_2 = 4 # m
I_1 = 0.123 # A = 123 mA
# ges: U_k_La_tat, P_La_tat
# Formel:
R_La = U_k_La/I_1
# R_l_1 = U_R_l_1/I_1
R_l_1 = (U_ges - U_k_La)/I_1
# Dreisatz
# 5 m = 1341.46 Ohm
# 4 m = x Ohm
R_l_2 = l_2 * R_l_1/l_1
R_ges_tat = R_l_2 + R_La
I_tat = U_ges / R_ges_tat
U_k_La_tat = R_La * I_tat
P_La_tat = U_k_La_tat * I_tat
# Ausgabe: print("U =", round(U, 4), "V")
print("R_La =", round(R_La, 4), "Ohm")
print("R_l_1 =", round(R_l_1, 4), "Ohm")
print("R_l_2 =", round(R_l_2, 4), "Ohm")
print("R_ges_tat =", round(R_ges_tat, 4), "Ohm")
print("I_tat =", round(I_tat, 4), "A")
print("U_k_La_tat =", round(U_k_La_tat, 4), "V")
print("P_La_tat =", round(P_La_tat, 4), "W")
# Lösung:
# 
```

    R_La = 528.4553 Ohm
    R_l_1 = 1341.4634 Ohm
    R_l_2 = 1073.1707 Ohm
    R_ges_tat = 1601.626 Ohm
    I_tat = 0.1436 A
    U_k_La_tat = 75.8883 V
    P_La_tat = 10.8979 W



```python

```
