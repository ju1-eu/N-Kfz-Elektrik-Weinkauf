# FM Nr. 5 Übungsaufgaben

## Innenwiderstand


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

**Aufgabe 1**

Ein 24 V Starter wird über zwei 12 V Batterien mit elektrischer Energie versorgt. Die Batteriezellen besitzen einen Innenwiderstand von $0,74~m\Omega$/Zelle. Durch die 2,3 m lange Versorgungsleitung mit einer Fläche von $120~mm^2$ fließt ein Strom von 1250 A. 

Wie groß ist die Klemmenspannung am Starter?

Skizze


```python
# Aufgabe 1
# geg: 
R_i_zelle = 0.00074 # Ohm = 0.74 mOhm/Zelle
U_Bat_1 = 12 # V
U_Bat_2 = 12 # V
z = 12 # Anzahl Batteriezellen
I = 1250 # A
l = 2.3 # m
A = 120 # mm^2
p = 0.0178 # Kupfer ohm x mm^2 / m 
# ges: U_K_st
# Formel:
# U_i = R_i_ges * I
U_i = R_i_zelle * z * I
U_v = I * p * l / A
# U_ges = U_i_ges + U_v + U_K_st
U_K_st = U_Bat_1 + U_Bat_2 - U_v - U_i
# Ausgabe: print("U =", round(U, 4), "V")
print("U_i =", round(U_i, 4), "V")
print("U_v =", round(U_v, 4), "V")
print("U_K_st =", round(U_K_st, 4), "V")
# Lösung:
# 
```

    U_i = 11.1 V
    U_v = 0.4265 V
    U_K_st = 12.4735 V



```python
# Aufgabe 2
# geg: Glühlampenaufschrift: 12 V / 4,5833 A
U = 12 # V
I = 4.5833 # A
U_q = 14.8 # V
R_i = 0.012 # Ohm = 12 mOhm
A_1 = 2 # mm^2
A_2 = 1 # mm^2
l_1 = 4.2 # m
l_2 = 1.5 # m
R_u = 0.050 # Ohm = 50 mOhm
p = 0.0178 # Kupfer ohm x mm^2 / m 
# ges: Mit welcher Klemmenspannung wird die Schaltung gespeist?
# Formel:
R_l_1 = p * l_1 / A_1
R_l_2 = p * l_2 / A_2
R_La = U / I
R_ges = R_i + R_l_1 + R_u + R_l_2 + R_La
I_tat = U_q / R_ges
U_K = U_q - I * R_i
# Ausgabe: print("U =", round(U, 4), "V")
print("R_l_1 =", round(R_l_1, 4), "Ohm")
print("R_l_2 =", round(R_l_2, 4), "Ohm")
print("R_La =", round(R_La, 4), "Ohm")
print("R_ges =", round(R_ges, 4), "Ohm")
print("I_tat =", round(I_tat, 4), "A")
print("U_K =", round(U_K, 4), "V")
# Lösung:
# 
```

    R_l_1 = 0.0374 Ohm
    R_l_2 = 0.0267 Ohm
    R_La = 2.6182 Ohm
    R_ges = 2.7443 Ohm
    I_tat = 5.393 A
    U_K = 14.745 V



```python

```
