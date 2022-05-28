# FM Nr. 1 Übungsaufgaben

## Ohmsches Gesetz Übung 1



**Aufgabe 1**

geg:
$R = 45~Ohm \quad
I = 0.32555~A$

ges: U in V

Lösung:
$U = R \cdot I =  14.6498~V$



```python
# Aufgabe 2
# geg:
U = 14.25 # V
I = 54.37 # A
# ges: R in Ohm
R = U/I
print("R = ", round(R, 4), "Ohm")
# Lösung: 
R =  0.2621 Ohm
```


```python
# Aufgabe 3
# geg:
U = 260 # V = 0.26 kV
R = 5000 # Ohm = 5 kOhm
# ges: I in A
I = U/R
print("I = ", round(I, 4), "A")
# Lösung: 
I =  0.052 A
```


```python
# Aufgabe 4
# geg:
R = 470 # Ohm
I = 0.03021 # A = 30,21 mA
# ges: U in V
U = R*I
print("U = ", round(U, 4), "V")
# Lösung:
U =  14.1987 V
```


```python
# Aufgabe 5
# geg:
U_1 = 14.82 # V 
R = 6.85 # Ohm 
# ges: I_delta in A
# U_1 = 14.82 = 100%
# U_2 = ?     =  60% (-40% Abnahme)
U_2 = U_1*60/100
I_1 = U_1/R
I_2 = U_2/R
I_delta = I_1 - I_2
print("I_1 = ", round(I_1, 4), "A")
print("I_2 = ", round(I_2, 4), "A")
print("I_delta = ", round(I_delta, 4), "A")
# Lösung: 
I_1 =  2.1635 A
I_2 =  1.2981 A
I_delta =  0.8654 A
```


```python
# Aufgabe 6
# geg:
U = 14.2 # V 
R_E12 = 2.618 # Ohm 
R_K2 = 72 # Ohm 
# ges: I_Steuer, I_F2 in A
I_Steuer = U/R_K2
I_F2 = U/R_E12
print("I_Steuer = ", round(I_Steuer, 4), "A")
print("I_F2 = ", round(I_F2, 4), "A")
# Lösung: 
I_Steuer =  0.1972 A
I_F2 =  5.424 A
```


```python
# Aufgabe 7
# geg:
I_delta = 4.32 # A 
R_kalt = 0.86 # Ohm 
U = 13.8 # V
# ges: I_kalt, I_warm in A, R_delta in Ohm
I_kalt = U/R_kalt
I_warm = I_kalt - I_delta
R_warm = U/I_warm
R_delta = R_warm - R_kalt
print("I_kalt = ", round(I_kalt, 4), "A")
print("I_warm = ", round(I_warm, 4), "A")
print("R_warm = ", round(R_warm, 4), "Ohm")
print("R_delta = ", round(R_delta, 4), "Ohm")
# Lösung: 
I_kalt =  16.0465 A
I_warm =  11.7265 A
R_warm =  1.1768 Ohm
R_delta =  0.3168 Ohm
```
