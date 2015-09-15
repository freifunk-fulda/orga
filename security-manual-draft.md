# Sicherheit in Freifunknetzen
## Sind unverschlüsselte WLANs wirklich unsicherer?
In den Medien wird es immer wieder propagiert und auch sonst überall hört man immer "Vorsicht vor offenen WLANs" oder "Achtung, verschlüsseln Sie ihr WLAN, damit Hacker keinen Zugriff darauf haben".

Falsch sind diese Aussagen nicht, soviel vorweg, aber das liegt eher daran, was sich in deinem Heimnetzwerk befindet.
Heutzutage kann so ziemlich alles WLAN haben.
Vom PC bis zum Toaster in der Küche.
Damit die auch das tun, was sie tun, ist ihr Primärziel erstmal untereinander zu kommunizieren und ggf. noch Updates von der Hersteller-Webseite beziehen.
Besonders die Kommunikation untereinander erfolgt innerhalb des eigenen Netzwerks häufig unverschlüsselt.
Man verlässt sich hier darauf, dass z.B. eben gerade das WLAN bereits verschlüsselt ist und nur vertrauenswürdige Geräte Zugriff haben.
Also zuhause das private WLAN verschlüsseln, ist in jedem Fall keine schlechte Idee.

Freifunk stellt aber kein Heimnetzwerk dar, sondern ein eigenes "kleines" Internet (ein sogenanntes Metronet also Stadtnetzwerk) mit Anbindung an das "große" Internet, welches sie auch so schon kennen. Der Unterschied ist hierbei, dass Freifunk sehr auf Regionalität und Freiheit setzt.
Es gibt keine klassischen Provider und es kostet auch nichts, Zugang zu erhalten, denn
schließlich können sie ihren Freifunkknoten auch ohne eigenen Internetanschluss betreiben und einfach nur über andere Freifunkknoten eine Verbindung zum Netzwerk aufbauen.
Die Gerätezielgruppe ist also etwas anders, als die in ihrem klassischen Heimnetzwerk.
Die meisten Clientgeräte innerhalb des Freifunknetzes sind Smartphones, Tablets und Laptops.
All dies sind Geräte, die sich oft auch so schon direkt im Internet befinden und somit auch nicht mehr oder weniger angreifbar sind also sonst.
Hiermit werden dann außerdem meist Webseiten aufgerufen, vielleicht ein wenig über Skype oder Mumble kommuniziert und über diverse Chat-Applikationen miteinander Nachrichten ausgetauscht.
Bei den gängigen Applikationen ist das offene WLAN also kein Problem.
Denn die meisten Verbindungen funktionieren über HTTPS.
Das S am Ende steht für Secure und bedeutet, dass die Kommunikation mit dem Webserver ohnehin verschlüsselt wird. unabhängig davon, ob sie sich in einem offenen oder verschlüsselten WLAN befinden. Und diese Verschlüsselung stellt für jeden Angreifer im WLAN erstmal eine ziemlich große Hürde da.
HTTPS-Webseiten erkennst du in allen gängigen Browser am Schlosssymbol in der Adresszeile.
Achte besonders dann auf das Schlosssymbol, wenn du Passwörter eingibst.
Nicht nur im Freifunknetzwerk, sondern überall.

Du fragst dich jetzt vielleicht, warum man Freifunk nicht einfach verschlüsselt und das Passwort z.B. auf die Flyer schreibt.
Das Problem ist: Selbst ein als sicher geltendes WPA2-PSK, welches du zuhause nutzt, ist eben nur so lange sicher, wie nur die Leute das Passwort kennen, die auch keine schlechten Absichten haben.
In Firmen sieht die Umgebung teilweise anders aus.
Wenn du aber z.B. in einem Café ein verschlüsseltes WLAN betrittst, bei dem alle das gleiche Passwort nutzen, bist du auch nicht sicherer als in einem unverschlüsselten Netzwerk, wie dem Freifunk Netz. Im Freifunk sparst du dir nur das Tippen des Passworts und kannst dich überall wo es Freifunk gibt problemlos bewegen ohne das WLAN wechseln zu müssen. ;)

Viele Firewall-Programme und auch die Windows-Firewall bieten für genau solche WLANs die Option des öffentlichen Netzwerks an.
Diese Einstellung ist empfohlen, da sie versucht alle unnötigen Zugriffe von außen zu blockieren.

Also alles in allem ist das Freifunk-Netzwerk eine sichere Sache, wenn man darauf achtet, dass die Firewall das Netzwerk als öffentliches ansieht und man darauf achtet HTTPS und TLS/SSL im Browser und für E-Mail Programme und andere Verbindungen zu benutzen.

## Dinge auf die man achten sollte, wenn man in offenen/fremden Netzwerken unterwegs ist

* Netzwerk als "öffentliches Netzwerk" in den Windows-Firewall Einstellungen markieren
* Freigaben von Daten ins Netzwerk abschalten
* HTTPS für alle Seiten, wo man sich anmeldet
* SSL/TLS in E-Mail Programmen aktivieren
* Bei Sicherheitswarnungen im Browser vorsichtig sein
* (optional) Verwenden von VPN

## Dinge die man in offenen/fremden Netzwerken vermeiden sollte

* Filesharing
* Öffnen von Ports
* "Firmen-/Heimnetzwerk"-Einstellungen in den Windows-Firewall Einstellungen nutzen
