---
title: 'Keywords'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!-----------------------------+
ju 19-3-22 Verbrennungsmotor-Abgasreduzierung
+------------------------------>
# Kraftstoffpumpenrelais 

**Nenne 3 Abschaltmöglichkeiten. Weshalb werden überhaupt das Kraftstoffpumpenrelais und damit die Kraftstoffförderpumpe abgeschaltet?**


1. **Konventionelle Abschaltung durch das Steuergerät**

    Bei Abstellung des Motors wird das Kraftstoffförderpumpenrelais vom SG nicht mehr angesteuert, somit wird kein Kraftstoff mehr gefördert.

2. **Ausfall des Bezugsmarken-Drehzahlgebers** 

    Fällt der *Bezugsmarken-Drehzahlgeber* aus, während des Betriebs oder bei Stillstand des Motors, kann das SG den ersten Zylinder nicht mehr zuordnen. Der Motor springt nicht mehr an. Ist dieses der Fall, schaltet das SG das Kraftstoffförderpumpenrelais ab. Mit dem Abschalten werden nachfolgende Komponenten nicht mehr mit Spannung versorgt:

   - Kraftstoffförderpumpe
   - alle Einspritzventile
   - Tankentlüftungsventil
   - Lambdasondenheizung

3. **Volllaufsicherung**

    Sollte der Motor durch ein unbeabsichtigtes Manöver des Fahrers einmal zum Stillstand gekommen sein, liefert der *Bezugsmarken-Drehzahlgeber* kein Signal mehr, aufgrund des stehenden Motors, an das SG. Sobald dieses Signal ausbleibt, schaltet das SG das Kraftstoffpumpenrelais ab, die Kraftstoffförderpumpe fördert keinen Kraftstoff mehr. 
    
    **Hintergrund**: Es kann ja sein, dass ein Einspritzventil undicht ist, das Einlassventil offen steht, somit würde, wenn die Kraftstoffförderpumpe weiterhin Kraftstoff fördert, in den entsprechenden Zylinder Kraftstoff eingespritzt. Er läuft also voll. Wird nun, nach einer Weile, wieder ein Startvorgang durchgeführt, kommt es zu einem kapitalen Folgeschaden, da nach dem *Pascalschen Gesetz*, Flüssigkeiten sich nicht zusammendrücken lassen. Die Folge wären mechanische Defekte am Kurbeltrieb und Kolben.

**Verunfallen** 

Kommt es zu einem Unfall, mit dem Auslösen des Airbags und anschließenden Überschlägen des Fahrzeugs, möchte man nicht, dass die Kraftstoffförderpumpe weiterhin Kraftstoff fördert. Es ist auch möglich, dass aus einer Kraftstoffleitung unkontrolliert Kraftstoff austritt, der sich unweigerlich an heißen Fahrzeugteilen, oder an Kurzschlussfunkenbildung entzünden würde. 

**Wann läuft die Kraftstoffpumpe an?** $\to$ über Türkontaktschalter



# Sekundärluftpumpe

Das **Sekundärluftsystem** wird bei Ottomotoren in der Kaltstartphase (3-5 Min.) aktiviert, um die Abgasbestandteile HC und CO in der Warmlaufphase zu minimieren, durch eine thermische Nachverbrennung.

**Sekundärluftpumpe** Umgebungsluft anzusaugen und diese in den Abgaskrümmer hinter den Auslassventilen einzublasen.

Durch Oxidation entsteht Wärme (unverbrannte Kohlenwasserstoffe reagieren mit Sauerstoff, Wärmeenergie wird frei)

*Ziel* 350 °C "light-off-Point" schnell erreichen.)

*Betriebstemperatur Katalysator*  650 bis 800 °C

# 3-Wege-Kat

**Welche Schadstoffe werden im Oxidationskatalysator zu welchen Stoffen umgewandelt?**

**Aufbau Katalysator** Keramik- o. Metallträger, Zwischenschicht (Wash-Coat, Oberfläche vergrößern), katalytisch aktive Schicht (Edelmetalle: Rhodium, Platin)

*Die chemischen Reaktionsgleichungen lauten:*

1. **Kohlenmonoxid** $CO$ + $O_2$ wird umgewandelt zu $CO_2$ = Kohlendioxid, Sauerstoff wird verbraucht

    - Katalysator = Platin $\to$ Oxidationsprozess 

2. **unverbrannte Kohlenwasserstoffe** $HC$ + $O_2$ werden umgewandelt zu $CO_2$ + $H_2O$ = Kohlendioxid und Wasser, Sauerstoff wird verbraucht

    - Katalysator = Platin $\to$ Oxidationsprozess

3. **Stickoxide** $NO_\text{x}$ wird umgewandelt zu $N_2$ + $O_2$, Sauerstoff wird freigesetzt

    - Katalysator = Rhodium $\to$ Reduktionsprozess


**Weshalb werden Oxidationskatalysatoren vor den Partikelfiltern eingebaut?**

Durch den Oxidationsprozess entsteht eine höhere Abgastemperatur, diese höhere
Abgastemperatur unterstützt die Regenration des Partikelfilters, das heißt, die Partikel können
dadurch abgebrannt werden.

# AdBlue

**Was ist an dem Motor anders? Warum braucht der Motor AdBlue?**

- höheres Verdichtungsverhältnis $\to$ weniger Kraftstoff notwendig
- höhere Wärme und Druck 
- mehr Stickoxide


AdBlue

- Reduktionsmittel
- gefriert - 11 °C
- 32,5 \% ca. 1/3 Harnstoff + 2/3 demineralisiertes Wasser (rein)

**chemische Prozess AdBlue** Hydrolysestrecke Harnstoff $\to$ Ammoniak (säurehaltig)
$\to$ SCR-Kat $\to$ $NO_\text{x}$ + Ammoniak umgewandelt in Stickstoff + Wasser

# Wie kann ich den Einsatz von Kraftstoff reduzieren? (Nacheinspritzung weglassen)

$\to$  Ausgangspunkt: Temperatur 550 °C notwendig

**Wie?**

- höherer Druck $\to$ höhere Temperatur 
- Ansauglufterwärmung (Kondensationsverluste reduzieren)
- Glühkerzen 
  - *Vorglühen* (Kaltstart)
  - *Zwischen glühen* (weniger Kraftstoff einsetzen)

# Schubabschaltung (Voraussetzung)

1. Drosselklappen geschlossen (Leerlaufkontakt) 
2. Kein Kraftstoff eingespritzt
3. Motortemperatur $>$ 80 °C 
4. Drehzahl $>$ wieder Einsetzdrehzahl (1400-1700 U/min)

# Schichtladebetrieb - homogene Gemischbildung

**Umschalten** erfolgt durch Gas geben: Schichtladebetrieb $\to$ homogene Gemischbildung

**Wie kann ich das klingeln vermeiden?**

$\to$ Ausgangslage Verdichtungsverhältnis bleibt konstant

$\to$ Brennraumtemperatur herabsetzen, wie?

1. **Zündzeitpunkt auf Spät verstellen,** d.h. 15° vor OT 
   - $\to$ Verbrennungshöchstdruck wird später erreicht, 20° nach OT 
   - Kolben wird weiter geschoben durch die vorhergehende Verbrennung
   - AV öffnet 148° nach OT, wir haben ein heißeres Abgas
     - $\to$ der Katalysator kommt schneller auf Betriebstemperatur
     - Wenn der Raum größer wird, nimmt der Druck ab und damit die Temperatur. (Hier nicht voll ausgenutzt, und damit habe ich ein heißeres Abgas)
   - **weniger Leistung** wird in Kauf genommen

2. **Kraftstoff Einspritzen**

    durch den Kraftstoff Einspitzen entziehe ich dem Verbrennungsprozess Wärme, dadurch wird die Brennraumtemperatur geringer, geringerer Druck und dadurch die Neigung zum Klingeln beseitigt

**Wärmekraftmaschine** 

Ottomotor / **Gleichraumverbrennung** / Kraftstoff-Luft Gemisch verdichten reicht nicht aus um einen sehr hohen Verbrennungsdruck und Temperatur zu bekommen, hier ist eine Zündkerze notwendig.

Vor Ende des Verdichtungstaktes 25-30° vor OT wird das komprimierte Kraftstoff-Luftgemisch fremdgezündet über den Funken der Zündkerze. (Entflammung)

Der Verbrennungshöchstdruck wird erreicht bei 3-6° nach OT, damit bekommt der Kolben ein auf den Deckel und geht nach unten.

**Höheres Verdichtungsverhältnis** (Nachteil) höhere Drücke $\to$ Kurbelwellenlager


# Lenkrollradius

**Fahrzeug mit Lenkrollradius Null bekommen in der Regel eine Lenkunterstützung eingebaut? (Hintergrund)**

Lenkrollradius = Lenkrollhalbmesser 

<!--27_FT_Lenkrollradius_Nachlauf vgl. abb.-->
![Lenkrollradius und Nachlauf](images/Skizze/27_FT_Lenkrollradius_Nachlauf.pdf){width=60%}

Bei einem **Lenkrollhalbmesser** $0$ trifft die Verlängerung der Lenkachse (Schwenkachse) mit der Mitte des Radaufstandspunktes in einem Punkt auf die Fahrbahn.

Erfordert **hohe Lenkkräfte** im Stand, Rad radiert auf der Stelle, Vorteil spurstabil.

Lenkrollhalbmesser wird bestimmt durch Sturz, Spreizung und Einpresstiefe der Felge.

**Negativer Lenkrollhalbmesser** wird bevorzugt 

- Vorteil Fahrzeug bleibt stabilisierend
- Flatterneigung
- Rad rollt um den Drehpunkt herum

Nachlauf (Teewagenprinzip)