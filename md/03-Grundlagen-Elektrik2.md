---
title: 'Grundlagen - Elektrik 2'
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
ju 24-3-22
+------------------------------>

# Potentialbestimmung 

<!--28_FT_Potentialbestimmung vgl. abb.-->
![Potentialbestimmung](images/Skizze/28_FT_Potentialbestimmung.pdf){width=60%}

Klemmenspannung und Potential

- $U_{R_1} = 3~V$, $U_{R_3} = 3~V$
- $U_{CE} = 6~V$, $U_{BA} = -3~V$, $U_{DA} = -9~V$

Möchte man das/ein Potential an einem Punkt in einem Stromkreis messen/bestimmen, bezieht man sich immer auf ein Bezugspotenzial. Die Schreibweise dieser Messung lautet dann zum Beispiel $U_{CE}$, hierbei möchte ich also das Potential C messen, C ist der erste Buchstabe, an ihm wird der *rote Clip* des Multimeters angeschlossen. Das Bezugspotenzial hierbei E ist der zweite Buchstabe, hier wird grundsätzlich der *schwarze Clip* des Multimeters angeschlossen. Potentialbestimmungen können auch zeichnerisch dargestellt werden. Hierbei lautet die Vereinbarung, die Pfeilspitze des Spannungs- oder Potentialpfeils trifft immer auf das Bezugspotenzial. Beispiel $U_{DA}$.

\newpage

# Brückenschaltung - Brückenspannung

<!--28_FT_Brueckenschaltung vgl. abb.-->
![Brückenschaltung](images/Skizze/28_FT_Brueckenschaltung.pdf){width=60%}

$U_{A\text{-}} = 6,9~V$, $U_{B\text{-}} = 6,9~V$, $U_{AB} = 0~V$ (keine Differenz)

$U_{A\text{+}} = -6,9~V$, $U_{B\text{+}} = -6,9~V$, $U_{AB} = 0~V$ (keine Differenz)

Poti $\to R_2 = 1~k$

$I_{Li} = \frac{U_{ges}}{R_{{Li}_{ges}}} = \frac{U_{ges}}{R_1 + R_2} = \frac{13,8}{5000 + 1000} =0,0023~A$

$U_{R_1} = R_1 \cdot I_{Li} = 5000~\Omega \cdot 0,0023~A = 11,5~V$

$U_{A\text{+}} = -11,5~V$, $U_{B\text{+}} = -6,9~V$, $U_{AB} = -4,6~V$

$I_{Re} = \frac{U_{R_3}}{R_3} = \frac{11,5}{12000} =0,00096~A$

$R_4 = \frac{U_{R_4}}{I_{Re}} = \frac{U_{ges} - U_{R_3}}{I_{Re}} = \frac{13,8 - 11,5}{0,00096} = 2395,83~\Omega$

\newpage

# Signalanlage Oldtimer (Prüfung)

**Aufgabe:** Stromlaufplan zeichnen

Ein Kunde beanstandet Folgendes:

**"Wenn ich den Fahrtrichtungsanzeiger setze und dabei das Bremspedal betätige, bleibt mein Fahrtrichtungsanzeiger stehen."** 

Lösen Sie dieses Problem mit einem entsprechenden Relaisschaltung. Komponenten, die vorhanden sein müssen: Batterie, 30/15/31ger Schiene, Blinkrelais (2-polig), Kontrollleuchte, Blinkerschalter, zwei Blinkleuchten links, zwei Blinkleuchten rechts. Dazu ein entsprechendes Relais.

**Problem - Spannungsverlust durch Bremse treten**

<!--29_FT_Signalanlage_Relais_6V vgl. abb.-->
![Signalanlage Oldtimer Relais](images/Skizze/29_FT_Signalanlage_Relais_6V.pdf){width=90%}




*Lösung* $\to$ Relais einbauen.

*Zündung Einschalten* Steuerstrom baut magnetisches Feld auf und schneidet die Spule, induziert dabei eine Spannung von $6~V$.

**Blinkfrequenz** $90 \pm30$ Impulse pro Minute

*Zündung ausschalten* Diode einbauen zwischen F4 und Anschluß 49

\newpage

# Tagfahrlicht verdrahten mit Relais Öffner oder Schließer

**Vorteile LED**

- Stromverbrauch 
- Haltbarkeit 
- Bezeichnung "RL" 
- Abstand $600~mm$

<!--29_FT_Tagfahrlicht_Relais vgl. abb.-->
![Tagfahrlicht Relais](images/Skizze/29_FT_Tagfahrlicht_Relais.pdf){width=90%}

**1) Wieso leuchtet das Tagfahrlicht ohne Standlicht?**
  - Das Relais ist hochohmig und das Standlicht (4x Lampen parallel) ist niederohmig. 
  - Das Relais holt sich die Masse über die Lampen.

**2) Was muss ich machen, damit ich Kraftstoff einsparen kann?**
  - Vgl. Abb. Tagfahrlicht
  - (1) Sicherung *F1* ziehen
  - (2) Sicherung *F1* und *F2* ziehen

\newpage
# Elektromotorarten

## Nebenschlussmotor 

Urmotor im Kfz, außer Starter

**Abk.**  | **Bezeichnung**
----------|-------------------------
$AW$      | Ankerwicklung (Spule)
$NSW$     | Nebenschlusswicklung (Spule)
$I_A$     | Ankerstrom
$I_{NSW}$ | Stromfluss durch die NSW
$RSW$     | Reihenschlusswicklung
$I_{RSW}$ | Stromfluss durch die RSW

**a) Nebenschlussmotor mit Feldwicklung** 

Kennlinie - Drehzahlverhalten

<!--30_FT_Nebenschlussmotor_mit_Feldwicklung vgl. abb.-->
![Nebenschlussmotor mit Feldwicklung](images/Skizze/30_FT_Nebenschlussmotor_mit_Feldwicklung.pdf){width=60%}

**b) Nebenschlussmotor mit Permanenterregung**

Kennlinie - Drehzahlverhalten

<!--30_FT_Nebenschlussmotor_mit_Permanenterregung vgl. abb.-->
![Nebenschlussmotor mit Permanenterregung](images/Skizze/30_FT_Nebenschlussmotor_mit_Permanenterregung.pdf){width=60%}

## Reihenschlussmotor 

Dreht hoch

Kennlinie - Drehzahlverhalten

<!--30_FT_Reihenschlussmotor vgl. abb.-->
![Reihenschlussmotor](images/Skizze/30_FT_Reihenschlussmotor.pdf){width=60%}

## Doppelschlussmotor 

Hohe Leistung

Kennlinie - Drehzahlverhalten

<!--30_FT_Doppelschlussmotor vgl. abb.-->
![Doppelschlussmotor](images/Skizze/30_FT_Doppelschlussmotor.pdf){width=60%}




## Wechselstrommotor 

Kennlinie - Drehzahlverhalten

<!--30_FT_Wechselstrommotor vgl. abb.-->
![Wechselstrommotor](images/Skizze/30_FT_Wechselstrommotor.pdf){width=60%}


## Schrittmotor 

Anwendung: Sitzverstellung, Scheinwerferhöhenverstellung, Schiebedach

Kennlinie - Drehzahlverhalten

<!--30_FT_Schrittmotor vgl. abb.-->
![Schrittmotor](images/Skizze/30_FT_Schrittmotor.pdf){width=60%}

## Drehstrommotor

Dozentenwechsel ...
