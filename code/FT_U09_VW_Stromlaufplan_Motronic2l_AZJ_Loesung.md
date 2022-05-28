# FT Nr. 9 Übungsaufgaben

## Aufgabenstellung Motronic 2,0l AZJ 

**Aufgabe 7**

```python
# geg:
U_B = 13,8 V
U_CE = 1,5 V
R_Ventil = 17 Ohm
# ges: P_E-Ventil_1.Zyl
# Formel:
I = U_Ventil / R_Ventil -> I = (U_B - U_CE) / R_Ventil
P = U x I -> P = (U_B - U_CE) x I
# Lösung:
I = 0,7235 A
P = 8,8994 W
```


**Aufgabe 8**


```python
# geg:
U_B = 13,8 V
U_CE = 1,5 V
R_Ventil = 17 Ohm
A = 0,35 mm^2 aus Stromlaufplan Nr. 77/9
l = 1,2 m
p = 0,0178 Ohm x mm^2/m
# ges: Spannungsminderung U_v_minusseitigeVersorgung_4.Zyl
# Formel:
U_Ventil = U_B - U_CE - U_v
R_l = p x l / A
R_ges = R_Ventil + R_l
I = U_k / R_ges -> I = (U_B - U_CE) / R_ges
U_v = I x R_l
# Alternative
U_v = I x p x l / A
# Lösung:
R_l = 0,061 Ohm
R_ges = 17,061 Ohm
I = 0,7209 A
U_v = 0,044 V
```
