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

