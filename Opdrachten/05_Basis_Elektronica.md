# Elektronica

In deze les kwamen we meer te weten over de basisprincipes en -componenten van elektronica. Voorbeelden hiervan zijn wat een stroomkring omvat, wat de grootheden zijn en hoe je ze kan berekenen, de verschillende apparatuur die je kan gebruiken, de verschillende componenten en het werken met schakelingen. Hierbij een synthese van de nota's die ik bij deze les maakte:

**Grootheden**

* **U** = spanning, uitgedrukt in volt V = verschil in potentiële elektrische energie tussen twee punten per eenheid van lading. 
* **R** = weerstand, uitgedrukt in ohm = elektrische eigenschappen van materialen om de doorgang van elektrische stroom te belemmeren > er komt dan een spanning over de weerstand te staan; lagere weerstand betekent betere geleiding.
* **I** = stroom, uitgedrukt in ampère A = transport van elektrische lading
* **P** = Vermogen, uitgedrukt in watt W = snelheid waarbij elektrische energie wordt verplaatst

Voornaamste berekeningen:
* U = R x I
* P = U x I
* P = U²/R

Als de spanning stijgt, dan stijgt de stroom.
Als de weerstand stijgt, dan daalt de stroom door de weerstand.
Als de stroom door de weerstand vergroot, dan stijgt de spanning over de weerstand.

**Apparatuur**

* Voeding
* Multimeter
* Oscilloscoop
* Functie generator

**Componenten**

* Weerstanden: twee geleidende draadjes waarrond koolstofbuisje met een bepaalde weerstand. De kleurcodes en hun positionering laten toe de waarde van de weerstand af te lezen. Er bestaan gewone en regelbare weerstanden, en er bestaan verschillende types van weerstanden: lichtgevoelige weerstanden (LDR), warmtegevoelige weerstanden (NTC negatieve temperatuur coëfficiënt, PTC), Flex (bijvoorbeeld bij e-textiles,…) en spanningsafhankelijke weerstanden.

* Bron: is de voeding en dus een belangrijk gegeven binnen een schakeling. 

* Schakelaars: bestaan in verschillende vormen en maten, aan te passen aan de toepassing. Voorbeelden: wisselschakelaar; normaal open schakelaar >< normaal gesloten schakelaar,…

* Spoel: is een geïsoleerde koperdraad omgewikkeld rond een bepaalde kern en gaat zich verzetten tegen alle verandering van de stroom (zal bijvoorbeeld als stroom wegvalt, ervoor zorgen dat de stroom toch blijft vloeien). Gaat een tegengestelde spanning opwekken en creëert hierdoor een soort elektromagneet (specifieke behandeling nodig omwille van het magnetisch veld). Zelfinductie, L - eenheid: Henry, H > impact van de spoel

* Condensator: bestaat uit twee platen met isolatie ertussen, waar geen stroom door kan, maar dat wel snel kan op- en ontladen. Bestaat in alle vormen en maten. Capaciteit, C - eenheid: Farad, F (meestal heel kleine waarden)

* Relais: bedienen van een schakelaar via een elektromagneet; wordt gebruikt voor heel grote en gevarieerde toepassingen.

* Diode: kan de stroom in één richting doorlaten > in de richting van de pijl. Anode (positief), kathode (negatief). Verschillende types: zenerdiode, schotkeydiode, photodiode.

* LED: "light emitting diode", vooral gemaakt om licht te maken. Afhankelijk van het kleur: verschillende spanning die nodig is voor de geleiding. 

* Transistor: stroomgestuurde schakelaar (complex).

* Mosfet: spanningsgestuurde schakelaar ("metal–oxide–semiconductor field-effect transistor"). Verschillende vormen en maten erin. Enhancement & N Channel. Grootte van de spanning die op de Gate komt, is van belang! Moet voldoende groot zijn, anders werkt het als een soort weerstand, zal warm worden,… VGS > Gate Threshold Voltage > mosfet als schakelaar, spanning op de gate naar de source moet groter zijn dan de threshold spanning van de gate naar de source om in geleiding te gaan.

* Spanningsregelaar: creëert een constante uitgangsspanning ongeacht de input (wel met limiet), bijvoorbeeld om een adruino, die 5V voeding nodig heeft, te laten werken met een batterij van 12V.

**Schakelingen**

Uitlezen van een schakelaar met Arduino. Ingang kan enkel zien of het signaal hoog is of laag; open schakelaar vormt een antenne die ruis kan oppikken > niet betrouwbaar:
* Pull down weerstand erbij schakelen: neutraliseert de ruis, trekt het naar de grond.
* Pull up weerstand: trekt het naar de 5V.

Bij Arduino: ofwel zelf weerstand bijschakelen; ofwel interne pull-up weerstand die aangezet kan worden in Arduino (interne poort activeren in de code, simpeler).

Ompoolbeveiliging: diode laat stroom in 1 richting toe te geleiden. Kan voorkomen dat project stuk gaat wanneer er te veel stroom doorgaat.

Bij het schakelen van een grote verbruiker > belangrijk om de gepaste mosfet te zoeken:
* Voldoende zwaar om spanning te onderbreken die je wilt kunnen onderbreken, VDS
* Moet stroom kunnen schakelen, ID
* RDS (on): weerstand, hoe lager hoe beter, minder spanningsveld en minder warm
* VGS (on): zo laag mogelijk, grootte van het stuursignaal

**Motoren** 

* DC motoren: simpele draaibeweging, niet zo precies en verbruiken veel stroom.
* Servo motoren: makkelijk aansturen met een arduino, elektronica zit er al ingebouwd in.
* Stappen motoren: kan stap per stap in alle richtingen draaien, heel nauwkeurig, bijvoorbeeld bij laser en 3D-printer. 

**Opdracht**

Als opdracht moesten we nadenken over een circuit dat aansluit bij ons project. Voorlopig ging ik hier nog niet mee aan de slag, aangezien ik geen plannen heb om elektronica te integreren in mijn eindwerk. 
