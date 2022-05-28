# FM Nr. 2 Übungsaufgaben

## Leiterwiderstand Übung 1


```python
# Aufgabe 1
# geg.:
l = 8.25 # m
A = 0.75 # mm^2
p = 0.0178 # Kupfer ohm x mm^2 / m 
# ges.: R_l
# Lösung
R_l = p*l / A
R_l =  0.1958 Ohm
```


```python
# Aufgabe 2
# geg.:
R_l = 3.648e-04 # Ohm = 0.3648 mOhm = 0.0003648 Ohm = 3.648e-04 Ohm
p = 0.0178 # Kupfer ohm x mm^2 / m 
d = 12.363 # mm
# ges.: l in m
# Lösung
# R_l = p*l / A
# pi/4 = 0.785
A = d**2 * 0.785
l = R_l * A / p
l =  2.459 m
```


```python
# Aufgabe 3
# geg.:
l = 4.5 # m
R_l = 0.00267 # 2,666666 mOhm  = 2,67e-03 Ohm
p = 0.0178 # Kupfer ohm x mm^2 / m 
# ges.: A
# Lösung
# R_l = p*l / A
A = p*l / R_l
A =  30.0 mm^2
```


```python
# Aufgabe 4
# geg.: Spule
d_m = 36 # mm = 3.6 cm
N = 1480 # Windungen
d_D = 0.36 # mm
p_cu = 8.93 # t/m^3 Dichte
p = 0.0178 # Kupfer ohm x mm^2 / m 
# ges.: l, A, R_l, G, V, m
# Lösung
# pi/4 = 0.785
# U = d * pi
# Kreisringfläche: d_mitte = d_m; D = Außendurchmesser; d = Innendurchmesser; r = Radius
# d_m = (D+d)/2; r_m = (D+d)/4
A = d_D**2 * ma.pi/4
#l = U * N [cm]
l = d_m/10 * ma.pi * N
R_l = p*l/100 / A
G = 1/R_l
#V = A * h [cm^3]
V = A/100 * l
m = V * p_cu
A =  0.1018 mm^2
l =  16738.4057 cm
R_l =  29.2711 Ohm
G =  0.0342 S
V =  17.0376 cm^3
m =  152.146 g
```


```python
# Aufgabe 5.1
# geg.:
R_l = 1.3171999e-2 # Ohm = 13.171999 mOhm = 0.013171999 Ohm = 1.3171999e-2 Ohm
p = 0.0178 # Kupfer ohm x mm^2 / m 
d = 1.784576526 # mm
# ges.: l in m
# Lösung
# R_l = p*l / A
# pi/4 = 0.785
A = d**2 * 0.785
l = R_l * A / p
l =  1.85 m
```

5.2) Gleiche Leiterfläche für die Rückleitung, dass sie genauso hoch belastet wird wie die positive Versorgungsleitung.

Sie liegen beide in Reihe, werden also vom gleichen Strom durchflossen.
