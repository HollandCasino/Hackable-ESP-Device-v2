Hints
=====
.. _hints:

Vind de root wachtwoord - Easy 
----------------
1. Schakel de full debug mode met een command.
2. Herstart het apparaat.
3. Kijk naar de startup bytes.

.. _hints2:

Schakel de ESP-LED uit/aan - Medium
-------------------
De hoofdpagina heeft een functie om de energie status in te stellen, dit regelt wat de LED doet. Bekijk de set_power functie, je kan ermee communiceren met 0 of 1. Als laatst Maak een HTML-document waarin jij de juiste URL aanroept, zodat elke keer een slachtoffer jouw webpagina gebruikt, jij als hacker hun LED controller kan bedienen.

.. _hints3:

Neem controle over de ESP-LED met een script - Medium
----------------------
De LED-controller heeft een oproepbare functie waarmee je de LED kunt bedienen.
1. Gebruik de URL-bibliotheek (urllib).  
2. Gebruik deze om een verzoek te doen met behulp van 'urlopen'.
3. Maak gebruik van de variabelen "state" en "addr" in de URL om de apparaten aan te roepen.
4. Onthoud, de code doet al de loop; je hoeft je alleen zorgen te maken over het maken van een "single call".

.. _hints4:

Vind de AES Keys - Medium
----------
1. Word een superuserop een van de twee manieren. Je moet eerst een superuser worden om de commandos te kunnen gebruiken.
2. Bekijk de commando's. Probeer verschillende commando's om de aes keys te vinden.

.. _hints5:

Word een superuser - Hard
--------------
1. Kijk naar de mogelijke commando's. Tip gebruik 'ls'.
2. Bekijk de bestanden met behulp van een commando.
3. De program pointer moet worden overschreven door de overflow.
4. Belangrijke regels in het programmabestand: 17, 19.
5. Belangrijke regel in het uit elkaar gehaalde programmabestand: 1, 27.
6. Probeer het programma uit te voeren met arguments, dit kan een paar pogingen duren.
7. De manier om hexidecimale waarden in te voeren is bijvoorbeeld: "\x11"

.. _hints6:

Upload een file in de website - Medium
-------------------------
Er is een configuratiebestand dat wordt gebruikt voor de webserver. Er zijn drie acties die kunnen worden uitgevoerd om twee informatiestukken te exploiteren.

1. Probeer de "user" pagina.
2. Heb je gekeken naar veelvoorkomende zwakke wachtwoorden?
3. Bekijk "config.conf".
4. Zoek naar het admin wachtwoord.
5. Probeer misschien in de seriële interface te kijken naar een manier om het bestand te decrypteren?
6. "gpg --decrypt key" is het juiste commando.
7. Het wachtwoord bevindt zich tussen de dubbele punten.
8. Er is een admin met een extra functie.
9. Probeer een bestand te uploaden?
