## Credential Bypass mit SQLi (Yven)
1. Um eine SQL Injection auf diesem Webshop zu machen kann man in den Komentären von Produkten suchen und dort einen Account unter den Kommentären finden. 
In diesem Fall sieht man sogar eine ganze Admin E-Mail adresse und somit kann man zum nächsten Schritt fortfahren

2. Auf der Login Page kann man zuerst ausprobieren ob die Seite überhaupt anfällig ist auf SQL Injections indem man beim Benutzernamen nur '- eingibt und beim passwort irgendetwas zufälliges.
Wenn dann etwas unerwartetes passiert wie zum Beispiel Error oder Object Object. Um weiter zu testen, kann man noch '-- eingeben und somit sollte es wieder "auskomentiert" sein und man sollte eine normale Fehlermeldung bekommen.
Um sich jetzt in den Webshop einzuloggen, muss man dann die ganze E-Mail beim Benutzernamen eingeben und am Ende der Email '--

## UNION JOIN Attack (Timothy)
1. SQLi Anfällige Angriffsvektoren finden (in diesem Fall sind es die Produktkategorien)
2. Produktkategorie Filter anwenden und ein ' am ende des URLs hinzufügen um nach einem Server error zu suchen. Einen weiteren hinzufügen um zu prüfen, dass kein weiteren Error erscheint.
3. '+UNION+SELECT+username,password+FROM+users-- am ende des URLs hinzufügen.
  - UNION SELECT: Kombiniert zwei SQL Abfragen von verschiedenen Tabellen. Die Abfrage muss dieselbe anzahl von select statements haben
4. Administrator credentials suchen und schlussendlich beim Login eingeben.
