# Meowduino
___
"Tiny paws, smart code."
___
**Author:** Ovejan Diana Elena

___

## Description

Acest proiect constă în transformarea unei jucării-pisică deja existente într-o pisicuță interactivă inteligentă, folosind o placă Arduino Nano și senzori de proximitate și atingere. Pisicuța reacționează la apropierea unei persoane prin mieunat, toarce și dă din coadă atunci când este mângâiată pe cap și se întinde pe lăbuțele din față când este apăsată pe una dintre ele.

___

## Motivation

Proiectul are ca scop combinarea elementelor de inginerie și interactivitate pentru a crea o jucărie inteligentă, empatică și simpatică, potrivită pentru persoanele care iubesc animalele, dar nu pot avea una reală (ex: alergii). Este, de asemenea, un proiect didactic care integrează cunoștințe din domeniile Arduino, senzori și electronică aplicată.

___

## Architecture

![image](https://github.com/user-attachments/assets/756857f3-0449-44af-8244-e8a006496792)



### Block Diagram

          [Ultrasonic Sensor HC-SR04]
                    ↓
               [Arduino Nano]
       ↙           ↓          ↘
[Capacitive Sensor] ↓       [Button]
                    ↓
        [Digital Logic (if/else)]
       ↙            ↓             ↘
 [Tone to Buzzer] [Motor Relay] [Purring Sound]
                         ↓
                      [DC Motor]


### Schematic (Textual)

Schematic (Textual)

D2 → Echo (ultrasonic)

D3 → Trigger (ultrasonic)

D4 → Capacitive Touch (simulat cu buton)

D5 → Paw Button

D6 → Relay control (DC motor)

D10 → Buzzer

Vin GND Arduino ↔ GND baterii externe

Motorul este alimentat prin 2 baterii AA de 1,5V fiecare, comutat prin releu

Diodă este conectată în paralel cu motorul (catod la +, anod la –) pentru protecție la tensiune inversă

## Components

| Device | Usage | Price (RON) | Link |
|-----------|-----------|--------------------|------|
| Placă de Dezvoltare Compatibilă cu Arduino Nano (ATmega328p și CH340) | Placă principală de control | 24.99 | [link](https://www.optimusdigital.ro/ro/compatibile-cu-arduino-nano/1686-placa-de-dezvoltare-compatibila-cu-arduino-nano-atmega328p-i-ch340.html) |
| Senzor Ultrasonic de Distanță HC-SR04+ | Detectează apropierea unei persoane | 14.99 | [link](https://www.optimusdigital.ro/ro/senzori-senzori-ultrasonici/2328-senzor-ultrasonic-de-distana-hc-sr04-compatibil-33-v-i-5-v.html) |
| Modul Senzor de Atingere Capacitiv TTP229 | Detectează mângâierea pe cap | 8.67 | [link](https://www.optimusdigital.ro/ro/senzori-senzori-de-atingere/1112-modul-senzor-de-atingere-capacitiv-ttp229.html) |
| Buton cu Capac Rotund Alb | Activarea lăbuțelor | 1.99 | [link](https://www.optimusdigital.ro/ro/butoane-i-comutatoare/1115-buton-cu-capac-rotund-alb.html) |
| Modul releu cu un canal (comandat cu 5 V) | Controlul motorului pentru coadă | 4.99 | [link](https://www.optimusdigital.ro/ro/electronica-de-putere-module-cu-releu/13084-modul-releu-cu-un-canal-comandat-cu-5-v.html) |
| Suport baterii 4 x R6 Pătrat | Alimentare Arduino și senzori | 5.33 | [link](https://www.optimusdigital.ro/ro/toate-produsele/2374-suport-baterii-4-x-r6-patrat.html) |
| Suport pentru Senzorul Ultrasonic HC-SR04 | Fixare senzor în corpul jucăriei | 3.49 | [link](https://www.optimusdigital.ro/ro/mecanica-accesorii-de-prindere/12246-suport-pentru-senzor-ultrasonic-hc-sr04.html) |
| Fire Colorate Mamă-Mamă (40p, 10 cm) | Conexiuni electrice | 6.99 | [link](https://www.optimusdigital.ro/ro/fire-fire-mufate/652-fire-colorate-mama-mama-40p-10-cm.html) |
| Fire Colorate Mamă-Tată (40p, 10 cm) | Conexiuni electrice mixte | 5.99 | [link](https://www.optimusdigital.ro/ro/fire-fire-mufate/653-fire-colorate-mama-tata-40p-10-cm.html) |
| Fire Colorate Tată-Tată (10p, 10 cm) | Conexiuni electrice | 5.70 | [link](https://www.optimusdigital.ro/ro/fire-fire-mufate/885-set-fire-tata-tata-10p-10-cm.html) |
| Kit Plusivo pentru Introducere în Electronică | Componente suplimentare (rezistori, LED-uri etc.) | 39.99 | [link](https://www.optimusdigital.ro/ro/kituri/12026-kit-plusivo-pentru-introducere-in-electronica-0721248990075.html) |
| Pisica Interactiva Albă cu Sunet & Lumină | Bază jucărie modificată în companion inteligent | 24.99 | [link](https://www.e-jumbo.ro/ro/jucarii/jucarii-bebelusi-prescolari/jucarii-prescolare-pentru-copii-6-luni/animale-interactive/animale-cu-mecanism-operate-cu-baterii/pisica-interactiva-alba-cu-sunet-lumina_1685254/) |

 **Total estimat:**  **~148.00 RON**

___

## Libraries

## Log

- **Week 6 – 12 May**: Achiziția componentelor
- **Week 7 – 19 May**: Asamblarea pieselor si programarea acestora
- **Week 8 – 26 May**: Finalizarea si prezentarea proiectului
