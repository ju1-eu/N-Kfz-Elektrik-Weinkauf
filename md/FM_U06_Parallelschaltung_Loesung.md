---
title: 'FM Nr.6 Übung'
author: ''
date: \today
subject: "Markdown"
keywords: [Markdown, Example]
lang: "de"
bibliography: literatur-kfz.bib 
csl: zitierstil-number.csl
---
<!--# FM Nr. 6 Übungsaufgaben
    Exponentialschreibweise: \num{2,67e-03} => 2.67 x 10^-3
    Pfeil: \curvearrowright  oder \to
    Mathemodus: https://katex.org/docs/supported.html
    13-2-22
-->
# Parallelschaltung Übung 6

**Aufgabe 1**

geg:

$R_1 = 72~\Omega, R_2 = 48~\Omega$
$R_{ges} = 12~\Omega$

ges: $R_3$

Formel:

$R_{ges} = \frac{1}{(\frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3})} \quad \to R_3 = \frac{1}{(\frac{1}{R_{ges}} - \frac{1}{R_1} - \frac{1}{R_2})}$

Lösung:

$R_3 = 20,5714~\Omega$


**Aufgabe 2**   


geg: ||

$R_1 = 30~\Omega, R_2 = 45~\Omega$

$I_1 = 0,45~A$

$I_{ges} = 0,8~A$

ges: $U, R_3, R_{ges}$

Formel:

$U = R_1 \cdot I_1$

$R_{ges} = \frac{U}{I_{ges}}$

$I_2 = \frac{U}{R_2}$

$I_{ges} = I_1 + I_2 + I_3 \quad \to I_3 = I_{ges} - I_1 - I_2$

$R_3 = \frac{U}{I_3}$

Lösung:

$U = 13,5~V$

$R_{ges} = 16,875~\Omega$

$I_2 = 0,3~A, I_3 = 0,05~A$

$R_3 = 270,0~\Omega$

\newpage

**Aufgabe 3**

geg:

$R_{Teil} = 66~\Omega$

$R_{ges} = 16,5~\Omega$

ges: $n$ (Anzahl)

Formel:

$R_{ges} = \frac{R_{Teil}}{n} \quad \to n = \frac{R_{Teil}}{R_{ges}}$

Lösung:

$n = 4$


**Aufgabe 4**

geg: ||

$R_2 = 3,4515~\Omega$

$I_1 = 0,85~A, I_2 = 4,23~A, I_3 = 1,85~A, I_4 = 2,69~A$

ges: $R_{ges}, R_1, R_4, R_3$

Formel:

$U = R_2 \cdot I_2$


$R_1 = \frac{U}{I_1}, R_3 = \frac{U}{I_3}, R_4 = \frac{U}{I_4}$

$I_{ges} = I_1 + I_2 + I_3 + I_4$

Variante 1: $R_{ges} = \frac{U}{I_{ges}}$ 
Variante 2: $R_{ges} = \frac{1}{(\frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3} + \frac{1}{R_4})}$ 

Lösung:

$U = 14,5998~V$

$R_1 = 17,1763~\Omega, R_3 = 7,8918~\Omega, R_4 = 5,4275~\Omega$

$I_{ges} = 9,62 A$

Variante 1: $R_{ges} = 1,5177~\Omega$
Variante 2: $R_{ges} = 1,5177~\Omega$ 

\newpage

**Aufgabe 5**


geg: || Glühkerze PTC Regelwiderstand $\theta$, x = Temperatur $\uparrow$, y = Widerstand $\uparrow$

$z = 4$ (Zylinderzahl)

$R_{R_k} = 0,38~\Omega$ (Regelwiderstand kalt)

$R_{R_w} = 0,88~\Omega$ (Regelwiderstand warm)

$R_H = 0,55~\Omega$ {Heizwendel}

$U_K = 13,8~V$

ges: $I_{{ges}_k}, I_{{ges}_w}, P_{K_k}, P_{K_w}$

Formel:

$I_{K_k} = \frac{U_K}{R_{K_k}} \quad \to I_{K_k} = \frac{U_K}{(R_{R_k} + R_H)}$

$I_{{ges}_k} = I_{K_k} \cdot z$

$I_{K_k} = \frac{U_K}{R_{K_w}} \quad \to I_{K_w} = \frac{U_K}{(R_{R_w} + R_H)}$

$I_{{ges}_w} = I_{K_w} \cdot z$

$P_{K_k} = U_K \cdot I_{K_k}, P_{K_w} = U_K \cdot I_{K_w}$

Lösung:

$I_{K_k} = 14,8387~A, I_{{ges}_k} = 59,3548~A$

$I_{K_w} = 9,6503~A, I_{{ges}_w} = 38,6014~A$

$P_{K_k} = 204,7742~W$ (Leistung - Glühkerze kalt)
$P_{K_w} = 133,1748~W$ (Leistung - Glühkerze warm)
