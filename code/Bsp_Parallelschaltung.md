# Rechenbeispiel - Parallelschaltung


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
# geg: ||
U = 13.5 # V Hinweis: U_ges = U
R_1 = 470 # Ohm
R_2 = 82 # Ohm
R_3 = 560 # Ohm
# ges: I_ges, I_1, I_2, I_3, R_ges
# Formel:
I_1 = U / R_1
I_2 = U / R_2
I_3 = U / R_3
I_ges = I_1 + I_2 + I_3
R_ges = U / I_ges
# Ausgabe: print("U =", round(U, 4), "V")
print("I_1 =", round(I_1, 4), "A")
print("I_2 =", round(I_2, 4), "A")
print("I_3 =", round(I_3, 4), "A")
print("I_ges =", round(I_ges, 4), "A")
print("R_ges =", round(R_ges, 4), "Ohm")
# Lösung:
# 
```

    I_1 = 0.0287 A
    I_2 = 0.1646 A
    I_3 = 0.0241 A
    I_ges = 0.2175 A
    R_ges = 62.079 Ohm



```python

```
