Das script1 wird im head ausgeführt und blockiert den Parsing Process es sollte daher am Ende des Bodys ausgeführt werden oder mit dem defer Attribut versehen werden um eine Verzögerung der Ladezeiten zu vermeiden.

Beobachtungen bei der Nutzung von defer und async

Nutzt man defer um script tag wird zuerst das inline script dann script2 und anschließend script1 ausgeführt
Nutzt man async so verändert sich die Reihenfolge es wird das inline script, dann script1 und anschließend script2 ausgeführt.
script3 wird on click ausgeführt.
