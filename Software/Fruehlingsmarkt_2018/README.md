# Glücksrad



**Allgemein**
-------------
- Preise
    - es gibt insgesamt 5 verschiedene Preiskategorien:
        - 1: 300x, blau
        - 2: 150x, grün
        - 3: 150x, rot
        - 4:  15x, gelb
        - 5:   5x, weiß
    - die Wahrscheinlichkeiten sind im besten Fall im Verhältnis von Anzahl zu Preissumme verteilt
- Buttons:
    - es gibt insgesamt zwei Buttons:
        - Bumper: extern am Glücksrad anzuschließender Riesenknopf
        - Mode:   kleiner, roter, an der Rückseite des Glücksrades befestigter Knopf



**Modi:**
---------
- Standard
    - die Preisverteilung entspricht den Standard-Werten und bleibt konstant
- Lenz
    - die Wahrscheinlichkeiten werden nach jedem Dreh neu entsprechend der Anzahl verbleibenden Preise verteilt
    - wenn alle Preise verteilt wurden (Summe der verbleibenden Preise = 0) wird dies durch eine Blink-Animation in den normalen Preisfarben kundgetan



**Drehen:**
-----------
- durch Drücken auf den Bumper im Demo-Modus wird die Dreh-Animation zu einem zufälligen Feld ausgelöst
- danach leuchten die LEDs in 3 verschiedenen Animationen (je nach Preisklasse) in der erdrehten Farbe auf
- während beider Vorgänge ist der Bumper blockiert
- durch drücken des Mode-Buttons wird die Animation beendet und der Bumper freigegeben


**Implementierungen**
---------------------
- [einfach](simple/README.md)
- [mit Menüstruktur](menu/README.md)