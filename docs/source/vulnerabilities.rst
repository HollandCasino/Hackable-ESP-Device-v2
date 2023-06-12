OWASP IoT Top 10 - Vulnerabilities
=====
De OWASP IoT Top 10 bestaat uit de volgende categorieën


- Weak, Guessable, or Hardcoded Passwords
- Insecure Network Services
- Insecure Ecosystem Interfaces
- Lack of Secure Update Mechanism
- Use of Insecure or Outdated Components
- Insufficient Privacy Protection
- Insecure Data Transfer and Storage
- Lack of Device Management
- Insecure Default Settings
- Lack of Physical Hardening
De volgende categorieën worden hier onder kort uitgelegd, en bij elke opdracht wordt hier de kwetsbaarheid uitgelegd.

I1 - Weak, Guessable, or Hardcoded Passwords
-------
Er is gebruikgemaakt van een makkelijke brute force, publieke beschikbare informatie of wachtwoorden die gemakkelijk te raden zijn. Ook is een backdoor in de firmware mogelijk of client software die ongeautoriseerde toegang verleent tot systemen die in gebruik zijn.

.. _vulnerabilities:

Vind de root wachtwoord - Serial leak (& web server users leak & encryption leak)
-------
De seriele console wordt vaak gebruikt bij het testen van software op microchips. De debug berichten kunnen gevoelige data bevatten zoals: gebruikersnamen en wachtwoorden. Dit apparaat heeft de mogelijkheid om verschillende commando’s te interpreteren. In dit geval wordt de seriële console niet uitgeschakeld voor de implementatie (deployment), wat kan leiden tot ernstige beveiligingsrisico’s. Vooral wanneer de commando’s kunnen worden uitgevoerd, is de data op het apparaat dan niet veilig.

I2 - Insecure Network services
-------
Onnodige of onbeveiligde netwerk services die op het apparaat runnen, vooral die blootgesteld zijn aan het internet, die de vertrouwelijkheid, integriteit/authenticatie, of beschikbaarheid van informatie in gevaar brengen. Of toegang tot ongeautoriseerde remote control. Een voorbeeld van een onveilige service kan zijn, een onveilige FTP-service in een IoT-apparaat dat gebruikmaakt van hardgecodeerde inloggegevens, door dat te misbruiken kan jij willekeurige gegevens lezen en schrijven op een apparaat.

.. _vulnerabilities2:
Schakel de ESP-LED uit/aan - Cross-site request forgery 
---------
Cross-site Request forgery is een aanval waarbij een gebruiker ongewenste acties kan uitvoeren op een webapplicatie. De applicatie waarmee jij de LED van de ESP-chip uit en aan kan zetten is kwetsbaar voor Cross-site request forgery (CSRF).

I3 - Insecure EcoSystem Interfaces
--------
Onveilige web, backend API, cloud, of mobiele interfaces in het ecosysteem buiten het apparaat kunnen ervoor zorgen dat het apparaat of de bijbehorende componenten gehackt kunnen worden. Veelvoorkomende problemen zijn onder andere het ontbreken van authenticatie/autorisatie, geen of zwakke versleuteling, en het ontbreken van het filteren van invoer (input) en uitvoer (output).

I4 - Lack Of Secure Update Mechanism
-----------------
IoT apparaten zijn meestal vaak goedkoop, energiezuinig en gebruiksvriendelijk ontworpen, wat kan leiden tot het missen van beveiligingsmaatregelen. Het ontbreken van een veilig update mechanisme maakt het IoT apparaat kwetsbaar en exploiteerbaar. Aanvallers kunnen misbruik maken van verouderde firmware of software om de beveiliging van het apparaat in gevaar te brengen.

I5 - Use Of Insecure or Outdated Components
---------------
Het gebruik van verouderde of onveilige softwarecomponenten/libraries die het apparaat kwetsbaar kunnen maken. Dit omvat onveilige aanpassingen aan besturingssystemen en het gebruik van software- of hardwarecomponenten van externe partijen uit een toeleveringsketen die aangetast is.

I6 -  Insufficient Privacy Protection
---------------
Veel IoT-apparaten verzamelen en bewaren gevoelige persoonlijke gegevens, maar missen vaak privacy/gegevensbescherming. De volgende kwetsbaarheden hebben gevolgen voor de privacy categorie: Seriële lekken, lekken van web server gebruikers, configuratie upload en download die exploiteerbaar zijn.
 
I7 - Insecure Data Transfer and Storage
---------
Het versturen en opslaan van data in plain tekst zonder encryptie is een groot probleem bij IoT apparaten. IoT apparaten verzamelen en slaan grote hoeveelheden data op. Aanvallers kunnen tijdens de overdracht (transfer van data) de gegevens onderscheppen, manipuleren of opslag mechanismen misbruiken.
De kwetsbaarheid van 4.1 is ook gerelateerd aan deze categorie.

I8 - Lack of Device Management
----------
Gebrek aan beveiliging, ondersteuning op apparaten die in productie zijn ingezet, inclusief asset management, updatebeheer, veilige buitenbedrijfstelling, systeembewaking en response mogelijkheden. Het gebrek aan device management kan voor ongeautoriseerde toegang zorgen, firmware tampering of device manipulation.

I9 - Insecure Default Settings
-----------
Apparaten of systemen die worden geleverd met onveilige standaardinstellingen of niet de mogelijkheid hebben om het systeem veiliger te maken door het beperken van de mogelijkheid voor operators om configuraties aan te passen.
De volgende kwetsbaarheden maken gebruik van enkele standaard en hard gecodeerde variabelen, waardoor ze telkens weer worden geleverd met dezelfde hard gecodeerde variabelen.



- Seriele lek
- lekken van webserver gebruikers
- versleuteling lek
- configuratie upload en download die exploiteerbaar zijn.

I10 - Lack of Physical Hardening
---------
Er is dus gebrek aan fysieke beveiliging in IoT-systemen. Het maakt de embedded devices kwetsbaar voor verschillende hardware aanvallen en firmware tampering, waardoor ongeauthoriseerde toegang mogelijk is voor aanvallers, een voorbeeld hiervan is root-seriele login, het extracten van gevoelige informatie enz. hierdoor zijn remote aanvallen en het overnemen van het apparaat mogelijk.
