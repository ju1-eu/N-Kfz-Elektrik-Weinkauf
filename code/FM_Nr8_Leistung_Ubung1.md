# FM Nr. x Übungsaufgaben

## x Übung 1


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
# Aufgabe 1
# geg:
U_ges = 14.8 # V
R_u = 0.05 # 50 mOhm
P_La = 55 # W
U = 12 # V
# ges: P_La_tat
# Formel:
# P_La = U x I -> P_La = U^2/R_La ->
R_La = U**2/P_La
R_ges = R_u + R_La
I_tat = U_ges/R_ges
# P_La_tat = U_k x I_tat ->
P_La_tat = R_La * I_tat**2
# Ausgabe: print("U =", round(U, 4), "V")
print("R_La =", round(R_La, 4), "Ohm")
print("R_ges =", round(R_ges, 4), "Ohm")
print("I_tat =", round(I_tat, 4), "A")
print("P_La_tat =", round(P_La_tat, 4), "W")
# Lösung:
# 
```

    R_La = 2.6182 Ohm
    R_ges = 2.6682 Ohm
    I_tat = 5.5468 A
    P_La_tat = 80.555 W



```python
# Aufgabe 2
# geg:
R = 50 # Ohm
P = 500 # W
# ges: I
# Formel:
# P = U x I -> P = R x I^2 -> 
I = ma.sqrt(P/R)
# Ausgabe: print("U =", round(U, 4), "V")
print("I =", round(I, 4), "A")
# Lösung:
# 
```

    I = 3.1623 A



```python
# Aufgabe 3
# geg:
U_ges = 12 # V
P_La = 21 # W
U_k = 8.6 # V
# ges: R_u, P_R_u, P_La_tat
# Formel:
# P_La = U x I -> P_La = U^2/R_La ->
R_La = U_ges**2/P_La
I_tat = U_k/R_La
# R_u = U_R_u/I_tat -> 
R_u = (U_ges - U_k)/I_tat
# P_R_u = U_R_u x I_tat ->
P_R_u = R_u * I_tat**2
P_La_tat = U_k * I_tat
# Ausgabe: print("U =", round(U, 4), "V")
print("R_La =", round(R_La, 4), "Ohm")
print("I_tat =", round(I_tat, 4), "A")
print("R_u =", round(R_u, 4), "Ohm")
print("P_R_u =", round(P_R_u, 4), "W")
print("P_La_tat =", round(P_La_tat, 4), "W")
# Lösung:
# 
```

    R_La = 6.8571 Ohm
    I_tat = 1.2542 A
    R_u = 2.711 Ohm
    P_R_u = 4.2642 W
    P_La_tat = 10.7858 W



```python
# Aufgabe 4
#geg:
P = 21 # W
U_1 = 12 # V
U_2 = 24 # V
# Formel:
# P = U x I -> P = U^2/R ->
R_1 = U_1**2/P
R_2 = U_2**2/P
Faktor = R_2/R_1
# Ausgabe: print("U =", round(U, 4), "V")
print("12V/21W R_1 =", round(R_1, 4), "Ohm")
print("24V/21W R_2 =", round(R_2, 4), "Ohm")
print("Faktor =", round(Faktor), "- fache Widerstand")
# Lösung:
# 
```

    12V/21W R_1 = 6.8571 Ohm
    24V/21W R_2 = 27.4286 Ohm
    Faktor = 4 - fache Widerstand



```python

```
