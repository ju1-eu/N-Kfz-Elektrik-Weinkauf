# FT Nr. 10 Übungsaufgaben

## Übungsaufgaben Beleuchtungssystem - Scheinwerferhöhenverstellung

**Aufgabe 10**

```python
# geg:
P_M_31 = 55 W/12V
U = 12 # V
U_ges = 14,3 V
U_v = 3,25 V
# ges: P_M_31_tat
# Formel:
P_M_31 = U x I -> I = P_M_31 / U
R = U / I
I_tat = U_k / R -> I_tat = (U_ges - U_v) / R
P_M_31_tat = U_k x I_tat -> P_M_31_tat = (U_ges - U_v) x I_tat
# Lösung:
I = 4,5833 A
R = 2,6182 Ohm
I_tat = 4,2205 A
P_M_31_tat = 46,6364 W
```



**Aufgabe 12**

```python
# geg:
P_12 = 21 W/12V
P_24 = 21 W/24V
U_12 = 12 V
U_24 = 24 V
# ges: R_24, R_12
# Formel:
P_12 = U x I -> I_12 = P_12 / U_12
R_12 = U_12 / I_12
P_24 = U x I -> I_24 = P_24 / U_24
R_24 = U_24 / I_24
Faktor = R_24 / R_12
# Lösung:
I_12 = 1,75 A
R_12 = 6,8571 Ohm
I_24 = 0,875 A
R_24 = 27,4286 Ohm
Faktor 12V / 24V = 4,0 -fache Leiterlaenge
```

