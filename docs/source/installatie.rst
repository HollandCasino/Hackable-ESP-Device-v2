Installatie instructie
=====
Voordat je begint aan de installatie zorg er voor dat je over de volgende software en hardware beschikt.

- Visual Studio Code.  (`Download <https://code.visualstudio.com/download>`_)
- 1x ESP32 Micro Controller. 
- 1x USB naar USB-Micro kabel.


[1] Installeer PlatformIO.
----------------
1. Open VSCode Extension Manager.

2. Zoek naar de PlatformIO IDE extentie.

3. Installeer `PlatformIO IDE <https://platformio.org/install/ide?install=vscode>`_.


[2] Installeren Git en clone van repository.
----------------

1. Ga naar https://git-scm.com/downloads en installeer de juiste versie voor jouw besturingssysteem.

2. Nadat Git is geïnstalleerd, open je VSCode.

We gaan nu de bestanden van het Hackable Device van GitHub clonen, zodat je ze kunt gebruiken. Voordat je met de volgende stappen begint, zorg ervoor dat je een map hebt gemaakt waarin je deze bestanden wilt opslaan.

3. Druk op Ctrl + Shift + P in VSCode.

4. Er wordt een zoekbalk geopend. Typ **"git clone"** en druk op Enter.

5. Nu verschijnt er **"Provide repository URL"**. Plak hier de onderstaande URL en druk op Enter.

- URL: https://github.com/pieterjm/hackable_esp_device

6. Je moet nu een map selecteren. Deze map heb je zojuist waarschijnlijk aangemaakt. Selecteer die map en klik vervolgens op **"Select as Repository Destination"**.

[3] PlatformIO gebruiken.
----------------
Je hebt nu de bestanden naar een map gecloned. Deze map met bestanden gaan we gebruiken.

1. Start VSCode en open binnen VSCode de map waar de geclonde bestanden in staan.

2. Links in de **"Explorer"** zie je onderaan het bestand **"toPlatformio.ps1"** staan. Klik op dit bestand en Run deze.

3. Het script start en vraagt om input. Typ **"C"** en druk op Enter. Het script gaat verder en druk daarna nogmaals op Enter.

De map **"HackableEspDevicePlatformio"** is nu aangemaakt. In de volgende stappen gaan wij deze gebruiken.

4. Open PlatformIO door in de zijbalk van VSCode op het Alien logo te klikken.

5. Onder **"Quick Access"** staat **"PIO Home"**, klik op de bovenstaande optie **"Open"**

6. Klik op **"Open Project"**, rechts in het scherm onder **"Quick Access"**

7. Ga naar de map met de geclonde bestanden en selecteer **"HackableEspDevicePlatformio"** (Die je in de eerste 3 stappen hebt aangemaakt)

8. Klik op **"Open HackableEspDevicePlatformio"**

[4] Flashen naar de ESP Controller.
----------------
1. Kijk onder **"Project Tasks"** naar **"General"** en klik op **"Upload"**.

2. Kijk onder **"Project Tasks"** naar **"Platform"** en klik op **"Upload filesystem image"**.

3. Nadat het programma klaar is in de terminal, klik onder **"General"** op **"Monitor"**.

[5] Access Point Connect
----------------

