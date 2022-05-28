---
title: 'VW-Stromlaufplan'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!---------------------------
Dozent: Horst Weinkauf
Thema:  VW Stromlaufplan lesen
Fachbuch ([@brand:2020:fachkundeKfz] S. 243)
Fachbuch ([@respondeck:2019:servicetechniker] S. 142)
Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)
#
## 
ju 3-3-22 
+------------------------------>

# Aufgabenstellung Messübungen Motronic 2,0l AZJ

**(Ü9) Aufgabenstellung und VW Stromlaufplan S. 1-3 Erklärung**

$\to$ vom Ziel zurück zur Batterie/Generator lesen

$\to$ Elektrische Ladungen gleichen sich grundsätzlich immer dort aus, wo sie getrennt worden sind!

$\to$ Ein elektrischer Strom kann grundsätzlich immer nur in einem geschlossenen Stromkreis fließen.

**Aufgabe 1**

Ja, die Aussage ist zutreffend. Strompfad 101-107
   
- S223 Sicherung im Strompfad 99, rot, 10 A 
- und S163 Sicherung Strompfad 8, rot 50 A 

*Farben der Sicherungen* Vgl. Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)

**Aufgabe 2**

S243 Sicherung Strompfad 156, über die Trennstelle T4f/1 Strompfad 112 erfolgt die positive Spannungsversorgung.

**Aufgabe 3**

Kl. 3/86 + auf Kl. 5/85 - messen, Bordnetzspannung beträgt 13,8 V

Die Spannung, die am Steuerstrom Anschluss gemessen werden kann, beträgt 4,6 V.

*Alternative:*  die Gesamtspannung durch die Anzahl der Widerstände dividieren. Hier in diesem Fall haben wir es mit drei gleich große Widerstände zu tun.

3x gleich große Widerstände a $72~\Omega \quad$ $U_{Teil} = \frac{13,8~V}{3} = 4,6~V$

**Aufgabe 4**

Ja, sie werden durch zwei verschiedene Sicherungen abgesichert.

- Komponente N156 S10 mit 15 A, Strompfad 19
- Komponente N261 S234 mit 10 A Strompfad 157

**Aufgabe 5**

Es wird gegen PIN1 und PIN4 jeweils ein positiver Spannungswert von 13,8 V gemessen (Bordnetzspannung), es fließt in der jetzigen Situation kein Strom, demzufolge kann auch an der Sicherung keine Spannung abfallen.
   
Das *Spannungsmessgerät* wird mit dem *roten Clip* an PIN1 kabelbaumseitig von G6, der *schwarze Clip* an PIN4 und PIN1 von G6 angeschlossen, es wird dann ein positiver Spannungswert angezeigt.


**Aufgabe 6**

Die Zündspule mit Leistungsendstufen im Strompfad 30 - 42 werden über die Trennstelle T6d/1 mit negativem Potenzial versorgt. Die Verbindung mit Masse erfolgt im Strompfad 180. 

Masseverbindung ist im Strompfad 180 auf Masse geschadet/gelegt.

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

**Aufgabe 9**

1. Steuerstrom Kraftstoffpumpenrelais J17 (grün)
   - Stromlaufplan S. 2,3,11,12,13,2
2. Steuerstrom Relais J299 für Sekundärluftpumpe (rot)
   - Stromlaufplan S. 2, ... , 11,12,13,5
3. Laststrom Relais J299 für Sekundärluftpumpe, Laststrom V101 (blau)
   - Stromlaufplan S. 2,12

**Aufgabe 10**

V101 - Motor für Sekundärluftpumpe

Das Bauteil ist durch die Sicherung S162 im Sicherungshalter/Batterie (50 A) abgesichert. Strompfad 6 Stromlaufplan S. 12.