+++
author = "DS"
date = 0001-01-01T00:00:00Z
description = ""
draft = false
slug = "cat-ethernet"
title = "CAT Ethernet"

+++


Terminologia di base
- host
- hub
- IPv4
- PAN - LAN - WAN
- default gateway
- CAN

A differenza dei collegamenti [CAN-J1939](35.228.152.175:80/can-j1939/) che lavorano su bus, le reti Ethernet sono di tipo *point-to-point* o *star*, con un dispositivo (host) che funge da accentratore (hub)  - (default gateway)

![point-to-point](http://35.228.152.175/content/images/2020/03/point-to-point.png)


Gli apparati collegati con la rete Ethernet comunicano sulla rete cosi' creata (LAN) con protocollo IPV4 usando indirizzi locali di tipo 165.26.78.x e 165.26.79.x definiti da CAT

I protocolli di trasporto usati sono UDP e TCP

Può coesistere anche una WAN (definita da cliente o da CAT)

Tipo di trasmissione dati Ethernet: 
    simplex (una direzione sola - es =TV via cavo)
    half duplex (due direzioni, uno alla volta  - es = Walkie tokie
    full duplex (due direzioni, trasmette e riceve contemporaneamente)
_______________________________________________________________________________

==CAT usa due tipi di Ethernet:==
   
   a 2 fili (solo full duplex) per:
   - B CAM
   - D6:Cx displays
   - A6 ECMS (A6:Nx, A6:Mx), PLE
    
   a 4 fili (full duplex - ma puo' passare in half duplex in caso di problemi)
   - service computers (to service with the machine)
   -A CAM Gen 1 and Gen 2
   -D6:Cx displays
   -A5 ECMs (A5:Nx, A5:Mx, etc.)
   -A6:Nx
   -Commercial off the shelf components (Cisco, Motorola, etc.)
   
![ethernet](http://35.228.152.175/content/images/2020/03/ethernet.png)

Eth 2 fili 
- velocità trasmissione 100BASE-T1 (100Mb/s)
- full duplex
- 1 coppia di cavi blu-bianco
- connettori + sottili, cavi non riparabili

Eth 4 fili
- velocità trasmissione combinata 10BASE-T (10Mb/s) and 100BASE-TX (100Mb/s)
- due coppie cavi arancio-bianco e verde-bianco
- connettori diversi (Deutsch, BR-44/49, BR-81, AMP, M12) riparabili

Cose da NON fare nei collegamenti di rete

> -Do not create a new routing for the patch cable. The replacement patch cable should only follow the existing harness and existing route for Ethernet.
> -Do not use excessively long cable. Only use patch cables noted that on the schematic for the circuit intended.
> -Do not modify the Ethernet cable length. Extra cable length should be bundled by using a figure-8.
> -Do not use smaller than recommended cable ties, only use 7K-1181 Cable Strap. Using other, smaller cable ties can deform the cable with pinch points and introduce issues into the system.
> -Do not install contact pigtails on Ethernet. If a contact has failed or is suspect, patch cable or harness replacement is required.
> -Do not modify the contacts. (The only modification allowed is installation of a Deutsch on a 4 wire Ethernet patch cable.)
> -Do not kink the Ethernet cable at the connector or in the cable. Kinks and sharp bends can be removed by properly routing and installing the Ethernet patch cables. Kinks may be introduced by overtightening the cable ties.
> -Do not add in excessive amounts of connectors. Using correct sized patch cables will keep interconnects to a minimum.
> -Do not introduce poor bundling. Correctly bundle the additional harness length into a figure-8. The additional length should be properly strapped in a neat and clean fashion.
> -Do not coil the cable as coiling will add significant noise to the system and degrade the signal. Extra length should be bundled in a figure-8 pattern.
> -Do not install connectors in vertical positions as water entry may occur. Connectors should be installed horizontally to allow water run off.
> -Do not place Ethernet patch cables near or around electrical noise sources (solenoid driver, injectors, electrical motor, high voltage, high current, etc.) Only use the original existing harness and existing route for Ethernet patch cables. Ethernet cables and connectors should be routed 300 mm (11.81 inch) away from noise sources.

Cosa si vede con ET:

![port-statistics](http://35.228.152.175/content/images/2020/03/port-statistics.png)



