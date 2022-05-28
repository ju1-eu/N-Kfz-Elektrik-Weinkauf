---
title: 'Grundlagen-Elektrik'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!---------------------------
Quelle: [(at)monk:2014:raspberry]

Einheiten: $5~cm$, $\cdot$, $\dots$, $\Omega$
$100^\circ\text{C}$  > 100°C
$80~\%$           > 80 %
$\boxed{E=mc^2}$

\sim = ~

Römische Zahlen \mathrm{I,II,III,IV}

Exponentialschreibweise: \num{2,67e-03} => 2.67 x 10^-3
Pfeil: \curvearrowright  oder \to
Mathemodus: https://katex.org/docs/supported.html

\quad
\bigl[\frac{V}{\Omega}\bigl] große eckige Klammern

\approx rund

https://johnbsmith.github.io/Typografie/LaTeX-Befehle.htm

https://de.wikibooks.org/wiki/LaTeX-Kompendium:_Sonderzeichen

Fussnote [^1]        
[^1]: <https://bw-ju.de/>    > \footnote{\url{https://bw-ju.de/}} 

![Logo](images/logo.pdf){width=60%}

Bild vgl. abb.    > (\autoref{fig:bild}). 
Tabelle vgl. tab. > (\autoref{tab:tabellen}). 
Kapitel vgl. kap. > (\autoref{sec:zusammenfassung}). 
Code vgl. code.   > (\autoref{code:halloweltex}). 

<https://bw-ju.de/> > \url{https://bw-ju.de/} 

+-----------------------------+
Dozent: Horst Weinkauf
Thema:  Grundlagen Elektrik
Fachbuch ([@brand:2020:fachkundeKfz] S. 243)
Fachbuch ([@respondeck:2019:servicetechniker] S. 142)
Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)
Mathebuch ([@elbl:2016:technMa])
#
## 
ju 17-2-22
+------------------------------>

# Die elektrische Spannung

**Spannung** $U \quad \text{[Volt]} \quad [V]$

*italienischer Physiker Alessandro Volta (1745-1827)*

**Einheit** | **Abk.** | **Zahl**  | **Exponentialschreibweise**
------------|----------|-----------|----------------------------
kilo V      | $[KV]$   | $1000~V$  | $\num{1,0e3}~V$
Volt        | $[V]$    | $1~V$     | $\num{1,0e0}~V$
milli V     | $[mV]$   | $0,001~V$ | $\num{1,0e-3}~V$

In einer Spannungsquelle, z. B. Drehstromgenerator, werden die unterschiedlichen Ladungen unter Energieaufwand (Drehbewegung, Magnetismus) voneinander getrennt.

Es bilden sich zwei Pole aus. 

- Negativer Pol: hier herrscht Elektronenüberschuss 
- Positiver Pol: Elektronenmangel 

Man spricht hierbei auch von dem Vorhandensein einer Potentialdifferenz.

Diese beiden Ladungen haben das Bestreben sich auszugleichen, dieses Ausgleichsbestreben bezeichnet man als elektrische Spannung.

**Messen**

Das Spannungsmessgerät wird grundsätzlich parallel zum Messobjekt geschaltet.

*Besonderheit*: Spannungsmessgeräte besitzen ein sehr hochohmigen Innenwiderstand (Impedanz).

\newpage

# Der elektrische Strom

**Strom** $I \quad \text{[Ampere]} \quad [A]$

*französischer Physiker André-Marie Ampère (1775-1836)* 

I = Intensität, International "Ampere"

**Einheit** | **Abk.**  | **Zahl**        | **Exponentialschreibweise**
------------|-----------|-----------------|----------------------------
kilo A      | $[KA]$    | $1000~A$        | $\num{1,0e3}~A$
Ampere      | $[A]$     | $1~A$           | $\num{1,0e0}~A$
milli A     | $[mA]$    | $0,001~A$       | $\num{1,0e-3}~A$
micro A     | $[\mu A]$ | $0,000001~A$    | $\num{1,0e-6}~A$
nano A      | $[nA]$    | $0,000000001~A$ | $\num{1,0e-9}~A$

Der elektrische Strom ist die gerichtete Bewegung von freien Elektronen. 
 
Ursache des elektrischen Stroms ist die elektrische Spannung. Elektrischer Strom kann nur im geschlossenen Stromkreis fließen. Ein Stromkreis besteht mindestens aus dem Spannungserzeuger, dem Verbraucher und den Leitungen.

Fuse (Sicherung: T = Träge, f = schnell, ff = superschnell)

**Messen**

Das Strommessgerät wird in Reihe zum Messobjekt geschaltet.

*Besonderheit*:

Strommessgeräte besitzen einen sehr niederohmigen Innenwiderstand.

\newpage

# Der elektrische Widerstand

**Widerstand** $R \quad \text{[Ohm]} \quad [\Omega]$

*deutsche Physiker Georg Simon Ohm (1789-1854)* 
 
resistor = Widerstand

**Einheit**    | **Abk.**    | **Zahl**         | **Exponentialschreibweise**
---------------|-------------|------------------|----------------------------
Mega $\Omega$  | $[M\Omega]$ | $1000000~\Omega$ | $\num{1,0e6}~\Omega$
Kilo $\Omega$  | $[K\Omega]$ | $1000~\Omega$    | $\num{1,0e3}~\Omega$
Ohm            | $[\Omega]$  | $1~\Omega$       | $\num{1,0e0}~\Omega$
milli $\Omega$ | $[m\Omega]$ | $0,001~\Omega$   | $\num{1,0e-3}~\Omega$

Bewegen sich Elektronen durch einen Leiter,  so prallen sie auf ihrem Weg durch den Leiter ständig mit den Atomen des Leiterwerkstoffes zusammen, sie werden also auf ihrem Weg durch den Leiter gehemmt. 
Dieses behindern der Ladungsträger bezeichnet man als elektrischer Widerstand.

<!--15_Schaltzeichen_Widerstand_Skizze vgl. abb.-->
![Schaltzeichen Widerstand](images/Skizze/15_Schaltzeichen_Widerstand_Skizze.pdf){width=30%}

<!--16_Widerstandsmessung_Skizze vgl. abb.-->
![Widerstandsmessung](images/Skizze/16_Widerstandsmessung_Skizze.pdf){width=60%}

**Messen**

Das Widerstandsmessgerät wird parallel zum Messobjekt geschaltet.

*Messvoraussetzung*:

Das Messobjekt muss aus dem Stromkreis heraus gelöst sein und sich im spannungsfreien Zustand befinden.

**Einsatzmöglichkeiten von Widerständen**

*Reihe*

(1) Strombegrenzung
(2) Spannungsteilung

*Parallel*

(1) Stromflusserhöhung
(2) Leistungsteilung $\boxed{R_{ges} = \frac{R_{Teil}}{n}}$ (z. B. $n = 2 \to$ Leistung halbieren)

<!--17_Leistungsteilung_Skizze vgl. abb.-->
![Leistungsteilung](images/Skizze/17_Leistungsteilung_Skizze.pdf){width=60%}

<!--18_Stromflusserhoehung_Strombegrenzung_Spannungsteilung_Skizze vgl. abb.-->
![Stromflusserhöhung, -begrenzung, Spannungsteilung](images/Skizze/18_Stromflusserhoehung_Strombegrenzung_Spannungsteilung_Skizze.pdf){width=60%}

\newpage

# Stromflussrichtungen

![Stromfluss und Messen](images/Skizze/06_Stromfluss_Messen_Skizze.pdf){width=60%}

**Technische Stromflussrichtung** der Strom fließt von plus nach minus

**physikalische Stromflussrichtung** tatsächlicher Elektronenfluss, die Elektronen bewegen sich von minus nach plus

\newpage

# Normgerechte Darstellung des Stromflusses durch einen Leiter


$\otimes$ Strom fließt vom Betrachter weg

$\odot$ Strom fließt auf den Betrachter zu

# Magnetfeld eines stromdurchflossenen Leiters

Magnetfeldrichtung festlegen

<!--Stromdurchflossener Leiter vgl. abb.-->

![Stromdurchflossener Leiter](images/Skizze/05_StromdurchflossenerLeiter_Skizze.pdf){width=60%}


# Normgerechte Festlegung des Nordpols einer stromdurchflossenen Spule

<!--Stromdurchflossene Spule vgl. abb.-->

![Stromdurchflossene Spule](images/Skizze/03_StromdurchflosseneSpule_Skizze.pdf){width=60%}


Umfasst man mit der rechten Hand eine stromdurchflossene Spule so, dass die Finger in Stromflussrichtung zeigen (technische Stromflussrichtung), so zeigt der abgespreizte Daumen in Richtung des Nordpols.

\newpage

# Rechte Hand-Regel (Generatorregel)

<!--Generatorregel vgl. abb.-->

![Generatorregel](images/Skizze/01_Generatorregel_Skizze.pdf){width=60%}



Hält man die rechte Hand so in ein Magnetfeld, sodass der Nordpol in die Handinnenfläche eintrifft. Und übt man dabei eine Bewegung in Richtung des abgespreizten Daumens aus, so fließt ein Strom in Richtung der Fingerspitzen.

# Linke Hand Regel (Motorregel)

<!--Motorregel vgl. abb.-->

![Motorregel](images/Skizze/02_Motorregel_Skizze.pdf){width=60%}


Hält man die linke Hand so in ein Magnetfeld, dass der Nordpol in die Handinnenfläche eintrifft und fließt dabei ein Strom in Richtung der Fingerspitzen, so wird der Leiter in Richtung des abgespreizten Daumens aus dem Magnetfeld abgelenkt.


# Das ohmsche Gesetz

Im ohmschen Widerstand sind die Beziehungen zwischen Strom, Spannung und Widerstand im Stromkreis festgelegt. Die Stromstärke steigt mit zunehmender Spannung und sinkt mit zunehmendem Widerstand.

$\boxed{I = \frac{U}{R}} \quad \bigl[\frac{V}{\Omega}\bigl] = A \quad
 \boxed{R = \frac{U}{I}} \quad \bigl[\frac{V}{A}\bigl] = \Omega \quad
 \boxed{U = R \cdot I} \quad [\Omega \cdot A] = V$

\newpage

# Stromdichte J

<!--Stromdichte vgl. abb.-->

![Stromdichte](images/Skizze/04_Stromdichte_Skizze.pdf){width=40%}

- **Große Fläche**
    - Kleine Stromdichte
- **Kleine Fläche**
    - Große Stromdichte

Unter Stromdichte versteht man die Anzahl der Ladungsträger Elektronen pro Flächeninhalt $mm^2$ . Die Stromdichte ist die Ursache der Erwärmung eines leitenden Stoffes. Ist die zu groß, wird oder kann der Leiter zerstört werden. 

**Erlaubte Stromdichte Werte:**

$J_{\text{zulässig}} = 10~\frac{A}{mm^2} \,\text{bei Kurzzeitbelastung}$

$J_{\text{zulässig}} = 30~\frac{A}{mm^2} \,\text{zugelassen (Starter)}$

**Formel**

$\boxed{J = \frac{I}{A}} \quad \bigl[\frac{A}{mm^2}\bigl] \quad
 \boxed{I = J \cdot A} \quad \bigl[\frac{A \cdot mm^2}{mm^2} = A\bigl] \quad
 \boxed{A = \frac{I}{J}} \quad \bigl[\frac{A \cdot mm^2}{A} = mm^2\bigl]$

# Leitwert G

Der Leitwert ist das Vermögen eines Widerstandes einen Strom fließen lassen zu können. Ein "hochohmiger Widerstand" lässt einen kleinen Stromfluss zu. Der besitzt also einen kleinen Leitwert. 
Und umgekehrt ein "niederohmiger Widerstand", lässt einen hohen Stromfluss zu. Der besitzt einen großen Leitwert. 
Der Leitwert ist der Kehrwert des Widerstandes.

**Formel** 

$\boxed{G = \frac{1}{R}} \quad \bigl[\frac{1}{\Omega} = S\bigl] \,\text{Siemens} \quad \boxed{R = \frac{1}{G}} \quad \bigl[\frac{1}{S} = \Omega\bigl]$

# Leiterwiderstand 

*Abhängig*

1. Leiterlänge $l~[m] \quad R_l \sim l$
1. Leiterfläche $A~[mm^2] \quad R_l \sim \frac{1}{A}$
1. Werkstoff - spezifische Widerstand $\rho~\text{(rho)}~\bigl[\frac{\Omega \cdot mm^2}{m}\bigl] \quad R_l \sim \rho$



*Aluminium* $\rho_{Al} = 0,0278~\frac{\Omega \cdot mm^2}{m}$ ist hochohmiger als *Kupfer* $\rho_{cu} = 0,0178~\frac{\Omega \cdot mm^2}{m}$.

**Leiterwiderstand R**

Er hängt von der Leiterlänge, vom spezifischen Widerstand und dem Leiterquerschnitt ab.

**Spezifische Widerstand $\rho$ (rho)**

Ist der Widerstand eines Leiters von $1~m$ Länge und $1~mm^2$ Querschnitt.

**Formel** 

$\boxed{R_l = \frac{\rho \cdot l}{A}} \, \bigl[\frac{\Omega \cdot mm^2 \cdot m}{m \cdot mm^2} = \Omega\bigl]
\boxed{A = \frac{\rho \cdot l}{R_l}} \, \bigl[\frac{\Omega \cdot mm^2 \cdot m}{m \cdot \Omega} = mm^2\bigl]
\boxed{l = \frac{R_l \cdot A}{\rho}} \, \bigl[\frac{\Omega \cdot mm^2 \cdot m}{\Omega \cdot mm^2} = m\bigl]$

\newpage

# Reihenschaltung von Widerständen

![Reihenschaltung - Widerstände](images/Skizze/07_Reihenschaltung_Widerstaende_Skizze.pdf){width=60%}

$\boxed{U = R \cdot I}$

Werden mehrere verschieden - große oder gleich große Widerstände in Reihe geschaltet, so fällt an jedem Widerstand nach Größe des Widerstands eine Spannung ab, die addiert die Gesamtspannung ergibt.

$\boxed{U_{ges} = U_{R_1} + U_{R_2} + U_{R_3} + \dots + U_{R_n}} \quad \bigl[V + V + V\bigl] = V$ 

Möchte man den Spannungsabfall an gleich großen in Reihe geschalteten Widerständen berechnen, kann nachfolgende Gleichung verwendet werden.

$\boxed{U_{teil} = \frac{U_{ges}}{n}} \quad \bigl[\frac{V}{1}\bigl] = V$

Die Stromstärke ist an jedem Punkt des Stromkreises gleich groß, d.h. durch jeden Widerstand fließt die gleiche Stromstärke.

$\boxed{I_{ges} = I_{R_1} = I_{R_2} = I_{R_3} = \dots = I_{R_n}} \quad \bigl[A = A = A\bigl] = A$ 


Der Gesamtwiderstand der Schaltung setzt sich aus der Addition der Teilwiderstände zusammen.

$\boxed{R_{ges} = R_1 + R_2 + R_3 + \dots + R_n} \quad \bigl[\Omega + \Omega + \Omega\bigl] = \Omega$ 

**Rechenbeispiel**


geg:

$U_{ges} = 13,8~V$

$R_1 = 220~\Omega, R_2 = 470~\Omega, R_3 = 180~\Omega$

ges: $R_{ges}, I, U_1, U_2, U_3$

Formel

$R_{ges} = R_1 + R_2 + R_3$

$I = \frac{U_{ges}}{R_{ges}}$

$U_1 = R_1 \cdot I, U_2 = R_2 \cdot I, U_3 = R_3 \cdot I$

Lösung:

$R_{ges} = 870~\Omega$

$I = 0,0159~A$

$U_1 = 3,4897~V, U_2 = 7,4552~V, U_3 = 2,8552~V$

\newpage

# Relais

**Arten** 

1. Spannungsrelais (Schließer, Öffner, Wechsler)
2. Stromrelais

**Aufgaben**

1. kleiner Spannungsabfall
2. kein Einfluss auf Verbraucher



## Spannungsrelais

<!--08_Relais_Skizze vgl. abb.-->
![Relais](images/Skizze/08_Relais_Skizze.pdf){width=70%}

**Ströme einer Relaisschaltung**

<!--09_Stroeme_einer_Relaisschaltung_Skizze vgl. abb.-->
![Ströme einer Relaisschaltung](images/Skizze/09_Stroeme_einer_Relaisschaltung_Skizze.pdf){width=40%}

- *Steuerstrom:* $50 - 200~mA$
- *Laststrom:* nach Verbraucher und Hersteller
- *Relaisspulenwiderstand:* $50 - 100~\Omega$ (ohne Schutzbeschaltung)

## Stromrelais

Anhängerdose Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 281)

**Schaltung einer Nebelschlussleuchte bei Anhängerbetrieb**

**Schaltung mit Anhänger**

<!--10_Stromrelais_Skizze vgl. abb.-->
![Stromrelais](images/Skizze/10_Stromrelais_Skizze.pdf){width=60%}

**Rechenbeispiel**

geg:

$R_{Sp} = 0,2~\Omega, R_{La} = 6,85~\Omega$

$U_{ges} = 14,2~V$

ges: $R_{ges}, I, U_{K_{Sp}}, U_{K_{La}}, P$

Formel

$R_{ges} = R_{Sp} + R_{La}$

$I = \frac{U_{ges}}{R_{ges}}$

$U_{K_{Sp}} = R_{Sp} \cdot I, U_{K_{La}} = R_{La} \cdot I$

$P = U_{K_{La}} \cdot I$

Lösung:

$R_{ges} = 7,05~\Omega$

$I = 2,0142~A$

$U_{K_{Sp}} = 0,4028~V, U_{K_{La}} = 13,7972~V$

$P = 7,79~W$

## Reedkontaktschalter, Reedrelais

Schaltzeichen Fachbuch ([@brand:2020:fachkundeKfz] S. 681)

<!--12_Reedkontaktschalter_Skizze vgl. abb.-->
![Reedkontaktschalter](images/Skizze/12_Reedkontaktschalter_Skizze.pdf){width=10%}

**Einsatzmöglichkeiten**

1. Füllstandsanzeige
   - Wischwasser
   - Kühlwasser
2. Glühkerzenausfallkontrolle
3. Geschwindigkeitssensor

## Schrittrelais, Stromstoßrelais (Stromsparen)

<!--11_Schrittrelais_Skizze vgl. abb.-->
![Schrittrelais](images/Skizze/11_Schrittrelais_Skizze.pdf){width=15%}

keine Prüfung

bistabiles Relais (BMW)

\newpage

# Spannungsverlust - Spannungsfall - Spannungsabfall (Prüfung)

$U_v = u$

Nennquerschnitt Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 280)

Klemmbezeichnung Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 273)

Spannungsfall Tabellenbuch ([@bell:2021:tabellenbuchKfz] S. 280)

<!--13_Spannungsverlust_Skizze vgl. abb.-->
![Spannungsverlust](images/Skizze/13_Spannungsverlust_Skizze.pdf){width=65%}

**Bezeichnung** | **Benennung**           | **Einheit**
----------------|-------------------------|------------
$U_{ges}$       | Gesamtspannung          | $[V]$
$U_v$           | Spannungsverlust        | $[V]$
$U_k$           | Klemmspannung           | $[V]$
$R_l$           | Leiterwiderstand        | $[\Omega]$
$I$             | Stromfluss, Stromstärke | $[A]$

$U_{ges} = U_v + U_k;\, U_k = U_{ges} - U_v;\, U_v = U_{ges} - U_k$

$U_v = R_l \cdot I; R_l = \frac{\rho \cdot l}{A} \quad \bigl[\frac{\Omega \cdot mm^2 \cdot m}{m \cdot mm^2}\bigl] = \Omega$

$U_k = U_{ges} - R_l \cdot I$

$\boxed{U_v = \frac{\rho \cdot l \cdot I}{A}} \quad \bigl[\frac{\Omega \cdot mm^2 \cdot m \cdot A}{m \cdot mm^2}\bigl] = V$

$U_{v_{~\%}} = \frac{U_v \cdot 100}{U_{ges}} \quad \bigl[\frac{V \cdot ~\%}{V}\bigl] = ~\%$

$\boxed{U_{v_{max}} = 0,5~V}$

$\boxed{\text{max. Leiterwiderstand} = 1~\Omega}$ (außer Starterhauptleitung)

**Spannungsfall** $U_v$ in einem stromdurchflossenen Leiter entsteht infolge des Leiterwiderstandes ein Spannungsfall, der sich am Verbraucher als Verlust auswirkt.

**Leiterquerschnitt** $A$ der Mindestquerschnitt einer Leitung richtet sich nach der Stromstärke, der Leiterlänge, dem spezifischen Widerstand des Leitermaterials und dem zulässigen Spannungsfall. Wegen der Erwärmung des Leiters muss gegebenenfalls die Stromdichte nachgeprüft werden.

\newpage

# Innenwiderstand von Spannungsquellen

<!--14_ Innenwiderstand_von_Spannungsquellen_Skizze vgl. abb.-->
![Innenwiderstand von Spannungsquellen](images/Skizze/14_ Innenwiderstand_von_Spannungsquellen_Skizze.pdf){width=60%}


**Bezeichnung**  | **Benennung**                           | **Einheit**
-----------------|-----------------------------------------|------------
$U_q$            | Quellspannung                           | $[V]$
$U_0 (U_{Null})$ | Leerlaufspannung                        | $[V]$
$U_k$            | Klemmenspannung (Last, mit Verbraucher) | $[V]$
$U_i$            | Spannungsabfall am Innenwiderstand      | $[V]$
$R_i$            | Innenwiderstand                         | $[\Omega]$
$R_a$            | Außenwiderstand                         | $[\Omega]$
$I$              | Stromfluss, -stärke                     | $[A]$


**Innenwiderstand** $R_i$ ist die Summe der Innenwiderstände der Zellen. Er ist u. a. von der Temperatur und dem Lade- beziehungsweise Entladezustand abhängig. Die Klemmenspannung $U_k$ der belasteten Batterie ist deshalb um den Spannungsfall niedriger als die Leerlaufspannung $U_0$.

$U_q = U_k + U_i \quad [V + V] = V$

$U_k = U_q - U_i \quad [V - V] = V$

$U_i = U_q - U_k \quad [V - V] = V$

$U_i = I \cdot R_i \quad [A \cdot \Omega] = V$

$U_k = I \cdot R_a \quad [A \cdot \Omega] = V$

$I = \frac{U_i}{R_i} \quad [\frac{V}{\Omega}] = A$

$I = \frac{U_k}{R_a} \quad [\frac{V}{\Omega}] = A$

$I = \frac{U_q}{R_{ges}} \quad [\frac{V}{\Omega}] = A$

$I = \frac{U_q}{R_i + R_a} \quad [\frac{V}{\Omega + \Omega}] = A$

$\boxed{U_k = U_q - I \cdot R_i} \quad [V - A \cdot \Omega \rightarrow V - V] = V$

$\boxed{R_i = \frac{U_i}{I}} \quad [\frac{V}{A}] = \Omega$

**Rechenbeispiel**

geg:

$U_q = 12~V, U_k = 9,6~V$

$R_a = 2,618~\Omega$ (Außenwiderstand)

ges: $I, R_i$

Formel:

$I = \frac{U_k}{R_a}$

$R_i = \frac{U_{R_i}}{I} \to R_i = \frac{(U_q - U_k)}{I}$

Lösung: 

$I = 3,6669~A$

$R_i = 0,6545~\Omega$

\newpage

# Parallelschaltung von Widerständen


<!--19_Parallelschaltung_Widerstaende_Skizze vgl. abb.-->
![Parallelschaltung von Widerstände](images/Skizze/19_Parallelschaltung_Widerstaende_Skizze.pdf){width=60%}



Werden mehrere verschiedene - oder gleich große Widerstände parallel geschaltet, so fließt durch jeden Widerstand, nach Größe des Widerstandes ein Strom, der addiert den Gesamtstrom ergibt.

$I_{ges} = I_{R_1} + I_{R_2} + I_{R_3} + \dots + I_{R_n} \quad [A + A + A] = A$

An jeden parallel geschalteten Widerstand liegt die gleiche Spannung an.

$U_{ges} = U_{R_1} = U_{R_2} = U_{R_3} = \dots = U_{R_n} \quad [V = V = V] = V$

Der Gesamtwiderstand ist stets kleiner als der kleinste Einzelwiderstand.

$R_{ges} = \frac{1}{\frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3} + \dots + \frac{1}{R_n}} \quad \bigl[\frac{1}{\frac{1}{\Omega} + \frac{1}{\Omega} + \frac{1}{\Omega}} = \frac{1}{\frac{1}{\Omega}} = \frac{1}{S}\bigl] = \Omega$

Möchte Mann/Frau den Gesamtwiderstand von gleich großen parallel geschalteten Widerständen berechnen, kann nachfolgende Gleichung angewendet werden.

$R_{ges} = \frac{R_{Teil}}{n} \quad \bigl[\frac{\Omega}{1}\bigl] = \Omega \quad \to n = \frac{R_{Teil}}{R_{ges}} \quad \bigl[\frac{\Omega}{\Omega}\bigl] = 1$ 

n = Anzahl der Widerstände (gleich große Widerstände)

$R_{ges} = \frac{R_1 \cdot R_2}{R_1 + R_2}$

$R_{ges} = \frac{1}{\frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}}$

$\to R_{1} = \frac{1}{\frac{1}{R_{ges}} - \frac{1}{R_2} - \frac{1}{R_3}} \quad \to R_{2} = \frac{1}{\frac{1}{R_{ges}} - \frac{1}{R_1} - \frac{1}{R_3}}  \quad \to R_{3} = \frac{1}{\frac{1}{R_{ges}} - \frac{1}{R_1} - \frac{1}{R_2}}$

**Rechenbeispiel**

geg: ||

$U = 13,5~V$ (Hinweis: $U_{ges} = U$)

$R_1 = 470~\Omega, R_2 = 82~\Omega, R_3 = 560~\Omega$

ges: $I_{ges}, I_1, I_2, I_3, R_{ges}$

Formel:

$I_1 = \frac{U}{R_1}, I_2 = \frac{U}{R_2}, I_3 = \frac{U}{R_3}$

$I_{ges} = I_1 + I_2 + I_3$

$R_{ges} = \frac{U}{I_{ges}}$

Lösung:

$I_1 = 0,0287~A, I_2 = 0,1646~A, I_3 = 0,0241~A$

$I_{ges} = 0,2175~A$

$R_{ges} = 62,079~\Omega$

\newpage

# gemischte Schaltung


<!--25_gemischte_Schaltung vgl. abb.-->
![gemischte Schaltung](images/Skizze/25_gemischte_Schaltung.pdf){width=60%}


$R_\mathrm{I} = R_1 + R_2$

$R_\mathrm{II} = \frac{1}{\frac{1}{R_\mathrm{I}} + \frac{1}{R_4}}$

$R_{ges} = R_\mathrm{II} + R_3$

Gemischte Schaltungen berechnet man, indem man sie in Reihen- und Parallelschaltungen zerlegt und Ersatzwiderstände bildet.

**Rechenbeispiel**

geg:

$R_1 = 56~\Omega, R_2 = 390~\Omega, R_3 = 180~\Omega, R_4 = 220~\Omega$

$U_{ges} = 13,8~V$

ges: $U_{Teil}, R_{Teil}, I_{Teil}, I_{{ges}}, R_{ges}$

Formel:


$R_I = R_1 + R_2$

$R_{II} = \frac{1}{\frac{1}{R_I} + \frac{1}{R_4}}$

$R_{ges} = R_{II} + R_3$

$I_{ges} = \frac{U_{ges}}{R_{ges}}$

$U_{R_3} = R_3 \cdot I_{ges}$

$U_{R_{II}} = R_{II} \cdot I_{ges}$

$I_{R_I} = \frac{U_{R_{II}}}{R_I}$

$I_{R_4} = \frac{U_{R_{II}}}{R_4}$

$U_{R_1} = R_1 \cdot I_{R_I}$

$U_{R_2} = R_2 \cdot I_{R_I}$

Lösung:


$R_I = 446~\Omega, R_{II} = 147,3273~\Omega$

$R_{ges} = 327,3273~\Omega$

$I_{ges} = 0,0422~A$

$U_{R_3} = 7,5887~V, U_{R_{II}} = 6,2113~V$

$I_{R_I} = 0,0139~A, I_{R_4} = 0,0282~A$

$U_{R_1} = 0,7799~V, U_{R_2} = 5,4314~V$

\newpage

# Die elektrische Leistung

$P$ (Power) Watt, $[W], [kW]$

*schottischer Ingenieur James Watt (1736-1819)*

Glühlampe $12~V/21~W$, Wärmestrahlerbeleuchtungskörper 



<!--26_Leistung_Gluehlampe vgl. abb.-->
![Leistung Glühlampe](images/Skizze/26_Leistung_Gluehlampe.pdf){width=12%}



$\boxed{P = U \cdot I} \quad [V \cdot A] = W$

$\boxed{U = \frac{P}{I}} \quad [\frac{W}{A} \to \frac{V \cdot A}{A}] = V$

$\boxed{I = \frac{P}{U}} \quad [\frac{W}{V} \to \frac{V \cdot A}{V}] = A$

**wenn $I$ fehlt** (Einsetzverfahren)

$P = U \cdot I \quad [V \cdot A] = W, \quad I = \frac{U}{R} \quad [\frac{V}{\Omega}] = A$

$P = U \cdot \frac{U}{R} \to \boxed{P = \frac{U^2}{R}} \quad [\frac{V \cdot V}{\Omega} \to A \cdot V] = W$

**wenn $U$ fehlt** (Einsetzverfahren)

$P = U \cdot I \quad [V \cdot A] = W, \quad U = R \cdot I \quad [\Omega \cdot A] = V$

$P = R \cdot I \cdot I \to \boxed{P = R \cdot I^2} \quad [\Omega \cdot A \cdot A \to V \cdot A] = W$

Die elektrische Leistung $P$ ist das Produkt aus Spannung $U$ und Strom $I$. 

**Anmerkung** die verschiedenen Leistungen der unterschiedlichen Verbraucher, in Schaltungen, addieren sich zur Gesamtleistung.

**Merke** halbe Spannung bedeutet nicht halbe Leistung und umgekehrt halbe Leistung bedeutet nicht halbe Spannung, die Leistung ändert sich im Quadrat. 

Bei der Berechnung an/von Wärmestrahlerbeleuchtungskörpern, zuerst den Widerstand berechnen.

