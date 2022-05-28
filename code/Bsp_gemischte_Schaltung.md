**Rechenbeispiel**


```python
# geg:
R_1 = 56 # Ohm
R_2 = 390 # Ohm
R_3 = 180 # Ohm
R_4 = 220 # Ohm
U_ges = 13.8 # V
# ges: U_Teil, R_Teil, I_Teil, I_ges, R_ges
# Formel:
R_I = R_1 + R_2
R_II = 1/(1/R_I + 1/R_4)
R_ges = R_II + R_3
I_ges = U_ges/R_ges
U_R_3 = R_3 * I_ges
U_R_II = R_II * I_ges
I_R_I = U_R_II/R_I
I_R_4 = U_R_II/R_4
U_R_1 = R_1 * I_R_I
U_R_2 = R_2 * I_R_I
# Lösung:
R_I = 446 Ohm
R_II = 147.3273 Ohm
R_ges = 327.3273 Ohm
I_ges = 0.0422 A
U_R_3 = 7.5887 V
U_R_II = 6.2113 V
I_R_I = 0.0139 A
I_R_4 = 0.0282 A
U_R_1 = 0.7799 V
U_R_2 = 5.4314 V
```
