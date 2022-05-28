# FM Nr. 6 Übungsaufgaben

## Parallelschaltung


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
R_1 = 72 # Ohm
R_2 = 48 # Ohm
R_ges = 12 # Ohm
# ges: R_3
# Formel:
# R_ges = 1 / (1/R_1 + 1/R_2 + 1/R_3)
R_3 = 1 / (1/R_ges - 1/R_1 - 1/R_2)
# Ausgabe: print("U =", round(U, 4), "V")
print("R_3 =", round(R_3, 4), "Ohm")
# Lösung:
# 
```

    R_3 = 20.5714 Ohm



```python
# Aufgabe 2
# geg: ||
R_1 = 30 # Ohm
R_2 = 45 # Ohm
I_1 = 0.45 # A
I_ges = 0.8 # A
# ges: U, R_3, R_ges
# Formel:
U = R_1 * I_1
R_ges = U/I_ges
I_2 = U/R_2
# I_ges = I_1 + I_2 + I_3
I_3 = I_ges - I_1 - I_2
R_3 = U / I_3
# Ausgabe: print("U =", round(U, 4), "V")
print("U =", round(U, 4), "V")
print("R_ges =", round(R_ges, 4), "Ohm")
print("I_2 =", round(I_2, 4), "A")
print("I_3 =", round(I_3, 4), "A")
print("R_3 =", round(R_3, 4), "Ohm")
# Lösung:
# 
```

    U = 13.5 V
    R_ges = 16.875 Ohm
    I_2 = 0.3 A
    I_3 = 0.05 A
    R_3 = 270.0 Ohm



```python
# Aufgabe 3
# geg:
R_Teil = 66 # Ohm
R_ges = 16.5 # Ohm
# ges: n (Anzahl)
# Formel:
# R_ges = R_Teil/n
n = R_Teil/R_ges
# Ausgabe: print("U =", round(U, 4), "V")
print("n =", round(n, 4), "")
# Lösung:
# 
```

    n = 4.0 



```python
# Aufgabe 4
# geg: ||
R_2 = 3.4515 # Ohm
I_1 = 0.85 # A
I_2 = 4.23 # A
I_3 = 1.85 # A
I_4 = 2.69 # A
# ges: R_ges, R_1, R_4, R_3
# Formel:
U = R_2 * I_2
R_1 = U / I_1
R_3 = U / I_3
R_4 = U / I_4
I_ges = I_1 + I_2 + I_3 + I_4
R_ges_1 = U/I_ges # (Variante 1)
R_ges_2 = 1 / (1/R_1 + 1/R_2 + 1/R_3 + 1/R_4) # (Variante 2)
# Ausgabe: print("U =", round(U, 4), "V")
print("U =", round(U, 4), "V")
print("R_1 =", round(R_1, 4), "Ohm")
print("R_3 =", round(R_3, 4), "Ohm")
print("R_4 =", round(R_4, 4), "Ohm")
print("I_ges =", round(I_ges, 4), "A")
print("Variante 1: R_ges_1 =", round(R_ges_1, 4), "Ohm")
print("Variante 2: R_ges_2 =", round(R_ges_2, 4), "Ohm")
# Lösung:
# 
```

    U = 14.5998 V
    R_1 = 17.1763 Ohm
    R_3 = 7.8918 Ohm
    R_4 = 5.4275 Ohm
    I_ges = 9.62 A
    Variante 1: R_ges_1 = 1.5177 Ohm
    Variante 2: R_ges_2 = 1.5177 Ohm



```python
# Aufgabe 5
# geg: || Glühkerze
z = 4 # Zylinderzahl
# PTC Regelwiderstand, x = Temp. steigt, y = Widerstand steigt
R_R_k = 0.38 # Ohm 
R_R_w = 0.88 # Ohm 
R_H = 0.55 # Ohm Heizwendel
U_K = 13.8 # V
# ges: I_ges_k, I_ges_w, P_K_k, P_K_w
# Formel:
# I_K_k = U_K/R_K_k
I_K_k = U_K/(R_R_k + R_H)
I_ges_k = I_K_k * z
# I_K_k = U_K/R_K_w
I_K_w = U_K/(R_R_w + R_H)
I_ges_w = I_K_w * z
P_K_k = U_K * I_K_k
P_K_w = U_K * I_K_w
# Ausgabe: print("U =", round(U, 4), "V")
print("I_K_k =", round(I_K_k, 4), "A")
print("I_ges_k =", round(I_ges_k, 4), "A")
print("I_K_w =", round(I_K_w, 4), "A")
print("I_ges_w =", round(I_ges_w, 4), "A")
print("P_K_k =", round(P_K_k, 4), "W")
print("P_K_w =", round(P_K_w, 4), "W")
# Lösung:
# 
```

    I_K_k = 14.8387 A
    I_ges_k = 59.3548 A
    I_K_w = 9.6503 A
    I_ges_w = 38.6014 A
    P_K_k = 204.7742 W
    P_K_w = 133.1748 W



```python

```
