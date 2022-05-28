---
title: 'Beleuchtungssystem'
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
ju 24-3-22 
+------------------------------>

# Übungsaufgaben Beleuchtungssystem

**(Ü10) Scheinwerferhöhenverstellung Beleuchtungssystem + VW Stromlaufplan** 

**Aufgabe 1** 

- Ist eine Wartung durchgeführt worden? 
- Ist die Glühlampe oder der Scheinwerfer gewechselt worden
- ist eine Motorwäsche durchgeführt worden
- unter welchen Bedingungen ist dieses Ereignis aufgetreten (Feuchtigkeit, Wetter) 
- Unfall (Quetschung der Leitungen, Übergangswiderstand bilden) 
- witterungsbedingte Einflussnahme



**Aufgabe 2**  Messung Strompfad 186-196 (Schaltplan VW - Scheinwerferhöhenverstellung Beleuchtungssystem) 

<!--28_Scheinwerferhoehenverstellung vgl. abb.-->
![Scheinwerferhöhenverstellung](images/Skizze/28_Scheinwerferhoehenverstellung.pdf){width=90%}


- Klemmenspannung Stellmotor messen
- Geberspannung Signal (hoch/runter) messen
- Synchronisierung der Höhenverstellung durchführen
- mit Diagnosetester Fehlerspeicher auslesen
- Sichtprüfung Stecker, Leitung, Sicherung, Mechanik

**Aufgabe 3** Ausgangszustand ist eine abgeglichene Brückenschaltungsspannung zwischen dem Potenziometer E102 und Potenziometern der Scheinwerfermotoren V48 und V49. Wird die Potentiometerstellung (Stellrad) an E102 geändert, ändert sich automatisch die Brückenspannung zwischen den beiden Komponenten {E102 und den Potis von V48 und V49}. 

Die Auswerteelektronik erfasst im Brückenspannungswert und steuert die Motoren V48 und V49 so lange mit der entsprechenden Polarität an, bis die Brückenspannung wieder den Wert Null Volt erreicht. Die Brückenspannung hat jetzt wieder ihren Ausgangswert (0 V), allerdings bei einer anderen Stellung  der Reflektoren.

Als Information über den Drehwinkelstand der Motoren, dienen die Potenziometer, deren Schleifer mit den Reflektoren verbunden sind. 
 
Das Bauteil, welches in der Regel verstellt wird, ist der Reflektor. 

Die Drehrichtungsänderung erfolgt über die Polaritätsänderung an den elektrischen Anschlüssen der Motoren.



**Aufgabe 4** Messobjekt (Poti E102) muss aus dem Stromkreis gelöst und spannungsfrei sein. 

Zur Messung des Wiederstandes Poti gemäß seiner Funktion bewegen/drehen/verändern alle Funktionen/Stufen durchschalten.

**Aufgabe 5** Fahrzeuge mit Xeon Scheinwerfersystemen müssen mit  einer 

1. automatischen Scheinwerferhöhenverstellungeinrichtung und 
2. mit einer Scheinwerferreinigungsanlage ausgestattet sein, 
3. bei Scheinwerfern mit Gasentladungslampen für Abblendlicht, wenn hierbei das Fernlicht eingeschaltet wird, muss das Abblendlicht in Funktion bleiben, also eingeschaltet bleiben

siehe §50 STVZO, Tabellenbuch D2S, D2R, D1S, D1R

Scheinwerferhöhenverstellung

- Manuell 
- Automatisch
- Dynamisch 
- Stichwort: Scheinwerferreinigungsanlage

**Aufgabe 6** 

- Die Geräte M29, M31, V48 und V49 sind schaltungstechnisch parallel geschaltet, wobei M29 über die Sicherung S21 abgesichert wird, insofern hier keine Spannungsminderung auftreten wird 
- die Geräte M31 T10c/7, V48 T10b/1, V49 T10c/1, als auch E102 erfahren die Spannungsminderung um 3,25 V (alles auf die Masseversorgung des jeweiligen Bauteils gemessen) 
- Der Stromkreis muss geschlossen sein, es muss ein Strom fließen, also Licht (Abblendlicht) einschalten!
- Einsteller E102 während der Messung betätigen

**Aufgabe 7**

Prüfzeichen und Bauartgenehmigung für Fahrzeugteile §21a, §22a

- **BRD** `~~~` 
- **EG** e1 
- **ECE** E1 (Prüfbuchstabe, Genehmigungsnummer, 1 = Deutschland, 2 = Frankreich)

**Aufgabe 8**

Stromlaufplan Nr. 73/2 + 73/12 + 73/8 + 73/15

1. (Farbe Rot) Leuchtweitenregulierungsverlauf 
2. (Farbe Blau) Laststrom Motoren Leuchtweiten 
3. (Farbe Grün) Stromverlauf Abblendlicht

\newpage

**Aufgabe 9**

Schaltbild

<!--29_FT_minusseitiger_Ubergangswiderstand vgl. abb.-->
![minusseitiger Übergangswiderstand](images/Skizze/29_FT_minusseitiger_Ubergangswiderstand.pdf){width=60%}


Es hat sich zwischen T10c/3 und der Masseverbindung im Leitungsstrang Strompfad 184 ein Übergangswiderstand gebildet, er liegt in Reihe zum V49. Dieser Widerstand mindert die Klemmenspannung des Motors V49, ferner bekommt die Brückenschalung des V49 unplausible Widerstandswerte. Man spricht hierbei von einem minusseitigen Übergangswiderstand. Der Spannungsverlust, der hierbei entsteht, bezeichnet man als einen minusseitigen Spannungsverlust.

**Bezeichnung** | **Benennung**
----------------|--------------------------------------
V49             | Scheinwerferhöhenverstellmotor rechts
T10c/5          | Anschluss Steuerung
T10c/1          | Plusversorgung
T10c/3          | Masse
$R_\text{ü}$           | Übergangswiderstand

\newpage

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

**Aufgabe 11**

d = 31, 56a, 56b, 58R (Scheinwerfer vorne rechts)

\newpage

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

Bei einer 24 V Glühlampe ist der Widerstand viermal größer (vierfache Leiterlänge) als bei einer 12 V Glühlampe.  Dieser Widerstand liegt hierbei an einer doppelten Spannung gegenüber der 12 V Spannung. Durch die doppelte Spannung und dem vierfachen Widerstand ergibt sich eine gleiche Leistung, bei gleicher Baugröße des Glaskolbens.
Um diesen Widerstand in die gleiche Glaskolbengröße hineinzubekommen, ist die Glühwendel mäanderförmig gefertigt, im Glaskolben verlegt.


**Aufgabe 13**

siehe Musterlösung