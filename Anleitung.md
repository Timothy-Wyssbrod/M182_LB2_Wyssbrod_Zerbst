## OWASP 
1. Um eine SQL Injection auf diesem Webshop zu machen kann man in den Komentären von Produkten suchen und dort einen Account unter den Kommentären finden. 
In diesem Fall sieht man sogar eine ganze Admin E-Mail adresse und somit kann man zum nächsten Schritt fortfahren

2. Auf der Login Page kann man zuerst ausprobieren ob die Seite überhaupt anfällig ist auf SQL Injections indem man beim Benutzernamen nur '- eingibt und beim passwort irgendetwas zufälliges.
Wenn dann etwas unerwartetes passiert wie zum Beispiel Error oder Object Object. Um weiter zu testen, kann man noch '-- eingeben und somit sollte es wieder "auskomentiert" sein und man sollte eine normale Fehlermeldung bekommen.
Um sich jetzt in den Webshop einzuloggen, muss man dann die ganze E-Mail beim Benutzernamen eingeben und am Ende der Email '--
