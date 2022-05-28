# Rechenbeispiel Stromrelais


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
# Rechenbeispiel
# geg:
R_Sp = 0.2 # Ohm
R_La = 6.85 # Ohm
U_ges = 14.2 # V
# ges: U_KSp, U_KLa, P
# Formel
R_ges = R_Sp + R_La
I = U_ges/R_ges
U_KSp = R_Sp * I
U_KLa = R_La * I
P = U_KLa * I
# Lösung: print("U = ", round(U, 4), "V")
print("R_ges = ", round(R_ges, 4), "Ohm")
print("I = ", round(I, 4), "A")
print("U_KSp = ", round(U_KSp, 4), "V")
print("U_KLa = ", round(U_KLa, 4), "V")
print("P = ", round(P, 4), "W")
# R_ges =  7.05 Ohm
# I =  2.0142 A
# U_KSp =  0.4028 V
# U_KLa =  13.7972 V
# P =  27.79 W
```

    R_ges =  7.05 Ohm
    I =  2.0142 A
    U_KSp =  0.4028 V
    U_KLa =  13.7972 V
    P =  27.79 W



```python

```
