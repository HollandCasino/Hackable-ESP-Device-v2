Walkthrough
=====
Voordat je aan de walkthrough begint moet je eerst hier naar kijken > `Setup <setup.rst>`_

Introductie
-------------
Dit is een walkthrough waarbij je leert hoe je een ESP-apparaat kunt hacken. De walktrough bevat 6 opdrachten met verschillende moeilijkheidsgraden. Het is belangrijk om te weten dat de letterlijke antwoorden niet in dit document staan. Het wordt aanbevolen om eerst de kwetsbaarheden te proberen te vinden door het apparaat te verkennen. Op deze manier kun je zien hoeveel kennis je al hebt, wanneer je vastzit kan je naar `hints <hints.rst>`_  gaan om tips te vinden, en bij `vulnerabilities <vulnerabilities.rst>`_ worden de kwetsbaarheden uitgelegd, misschien kan je daar ook handige informatie vinden om de kwetsbaarheden te exploiteren.

Vind de root wachtwoord - Easy 
-----------
Jouw doel is om de root wachtwoord te vinden. Het apparaat maakt gebruik van een seriele console waarop debugberichten worden weergegeven.  Dit apparaat heeft de mogelijkheid om meerdere commando's te interpreteren. 
Kijk hier voor uitleg over de `kwetsbaarheid <vulnerabilities.rst#vulnerabilities>`_.
Kijk hier voor `Hints <hints.rst>`_

Schakel de ESP-LED uit/aan - Medium
------------
De website die je gebruikt is kwetsbaar voor Cross-site request forgery (CSRF) uitleg hier:  `CSRF <vulnerabilities.rst#vulnerabilities2>`_. Aan jou de taak is om een kwaadaardige HTML-pagina te maken. De webpagina moet de ESP op het juiste IP-adres oproepen en je moet een optie maken, waarmee de LED aan of uit gaat wanneer je de HTML-pagina opent.
`Hints <hints.rst>`_ 

Neem controle over de ESP-LED met een script - Medium
-------------
De LED-controller heeft een functie die oproepbaar is, waarmee jij controle hebt over de LED lichten. In deze challenge is jouw doel om controle te krijgen over de ESP en de LED lichten te manipuleren. Er staat een script in de github die 'BotLED_skel.py' heet. De control functie mist dus die moet jij zelf erin programmeren.

Vind de AES Keys - Medium
----------
CBC-modus is een AES-blokversleuteling-modus, waarbij het eerste plain tekstblok wordt gecombineerd met een initialisatievector voordat het wordt versleuteld. De decryptie werkt op dezelfde manier met gecodeerde (ciphered) tekst. Deze kwetsbaarheid gaat over het vinden van de sleutel en het decrypten van het bestand ermee.

Word een superuser - Hard
--------------
Vroeger kwamen buffer overflows vaak voor. Tegenwoordig zijn de meeste software zo geschreven dat een buffer overflow niet meer mogelijk is. Bij microchips zoals een ESP-apparaat kunnen buffer overflows nog steeds voorkomen. Een buffer overflow treedt op wanneer de hoeveelheid gegevens groter is dan de opslagcapaciteit van de memory buffer. Als gevolg hiervan probeert het programma dat de gegevens naar de buffer schrijft, per ongeluk aangrenzende geheugenlocaties overschrijden.
Bijvoorbeeld een buffer voor inloggegevens kan ontworpen zijn om gebruikersnaam en wachtwoord inputs van 8 bytes te verwachten, dus als er een transactie is met een invoer van 10 bytes, kan het programma de overtollige gegevens voorbij de buffergrens schrijven.
Als de transactie executable code overschrijft, kan dit ervoor zorgen dat het programma zich onvoorspelbaar gedraagt en kan het leiden tot onjuiste resultaten, geheugentoegang fouten (memory access errors), of crashes. Als de aanvallers de geheugenindeling van programma's kennen, kunnen ze inputs genereren die de buffer niet kan opslaan, waarbij ze deze vervangen door hun eigen code. Bijvoorbeeld: een aanvaller kan de program-pointer (een object dat naar een ander geheugenbereik wijst) en deze richten op een exploit-payload, om zo controle over het programma te krijgen. Jouw doel is om dus superuser te worden zonder een wachtwoord.


Upload een file in de website - Medium
-------------------------
Er is een configuratiebestand ergens verborgen op de webserver. Deze configuratie kan geback-upt en hersteld worden. Het back-uppen en herstellen is niet op de juiste manier beveiligd. Probeer hier misbruik van te maken.
