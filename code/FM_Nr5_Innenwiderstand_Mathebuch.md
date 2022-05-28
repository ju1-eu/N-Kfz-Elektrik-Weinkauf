---
title: 'FM Nr.5 Übung'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown, Example]
lang: "de"
bibliography: literatur.bib 
csl: zitierstil-number.csl
---
<!--# FM Nr. 5 Übungsaufgaben -->
# Innenwiderstand Übung 5 Mathebuch S. 121

**Aufgabe 1**

```python
# geg:
U_q = 12.6 # V
R_i = 0.012 # Ohm = 12 mOhm
R_a = 0.051 # Ohm
# ges: I, U_k
# Formel:
I = U_q/(R_i + R_a) # I = U_q/R_ges
U_k = I * R_a
# Ausgabe: print("I =", round(I, 4), "A")
print("I =", round(I, 4), "A")
print("U_k =", round(U_k, 4), "V")
# Lösung:
# I = 200.0 A
# U_k = 10.2 V
```

**Aufgabe 2**

```python
# geg:
I = 400 # A
U_q = 12.5 # V
U_k1 = 8.3 # V (nach 30s)
U_k2 = 6.2 # V (nach 150s)
# ges: R_i1, R_i2
# Formel:
R_i1 = (U_q - U_k1)/I # R_i1 = U_i1/I
R_i2 = (U_q - U_k2)/I # R_i2 = U_i2/I
# Lösung:
R_i1 = 0.0105 Ohm
R_i2 = 0.0158 Ohm
```

