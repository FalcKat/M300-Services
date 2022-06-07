# Docker 
## Was ist Docker?

Docker bzw. die Docker-Technologie ist eine Open-Source-Technologie. Im Kern wird sie für die Entwicklung, den Vertrieb und die Ausführung von Anwendungen verwendet.

Mit Docker können Sie Anwendungen von einer lokalen Infrastruktur isolieren. So ist die Softwarebereitstellung schneller, einfacher und sicherer als je zuvor.

## Welches sind die Kerneigenschaften?

Die Kerneigenschaft von Docker besteht darin, dass Anwendungen gekapselt in sogenannten Docker-Containern verpackt sind. Sie sind so für jedes System einzusetzen, auf dem ein Linux-, Macintosh- oder Windows-Betriebssystem ausgeführt wird. Seit längerer Zeit gibt es auch andere Containersysteme. Docker wurde jedoch populär, weil es eine leichter zugängliche und umfassendere Schnittstelle für diese Technologie bietet. Zudem wurde eine öffentliche Softwarequelle mit Basis-Container-Images geschaffen. Benutzer können auf ihr aufbauen, wenn sie containerisierte Umgebungen zur Ausführung ihrer Anwendungen erstellen.

## Was ist der Hauptvorteil von Docker?

Mit Docker können Sie sicherstellen, dass die Funktionalität Ihrer Anwendungen in jeder Umgebung ausgeführt werden kann. Dieser Vorteil entsteht, weil alle Anwendungen und deren Abhängigkeiten in einem Docker-Ausführungscontainer zusammengeführt werden.

Das bedeutet auch, dass z.B. DevOps-Profis (Development und IT-Operations) verschiedenste Anwendungen mit Docker generieren. Dadurch stellen sie sicher, dass sie sich nicht gegenseitig stören. Es können Container erstellt werden, auf dem verschiedene Anwendungen installiert sind. Der Container kann dann der Qualitätssicherung übergeben werden. Diese muss anschließend nur den Container ausführen, um sämtliche Abläufe und Funktionen systemunabhängig zu testen. Daher spart die Verwendung von Docker-Tools Zeit. Im Gegensatz zur Verwendung von Virtuellen Maschinen (VMs) müssen Sie sich keine Gedanken darüber machen, welche Plattform Sie verwenden:

Docker-Container funktionieren überall.

## Was genau ist ein Docker-Container?

Ein Docker-Container ist eine Standardsoftwareeinheit, die einen Code in all seinen Abhängigkeiten speichert. So wird die Anwendung schnell und zuverlässig auf verschiedensten Computerumgebungen lauffähig. Ein Docker-Container bildet ein leichtes eigenständiges ausführbares Softwarepaket ab, das alles enthält, was zum Ausführen einer Anwendungscodelaufzeit benötigt wird:

    Programmcode
    RunTime-Engines
    Systemtools
    Systembibliotheken
    Einstellungen

Diese Containerisierte Software läuft auf Linux-, Mac- und Windows-basierten Systemen unabhängig von der Infrastruktur immer gleich. Die Docker-Container isolieren die Software von der Umgebung und stellen sicher, dass sie trotz Unterschieden einheitlich funktioniert.

## Was sind die Vorteile von Containern?

Docker-Container sind besonders beliebt, weil sie gegenüber Virtuellen Maschinen (VMs) viele Vorteile bieten. VMs enthalten grundsätzlich vollständige Kopien eines mächtigen Betriebssystems, die Anwendung selbst, alle erforderlichen Binärdateien und Bibliotheken. Dies beansprucht in der Regel Dutzende von Gigabytes an Speicherkapazität. VMs können im Gegensatz zu Docker-Containern auch nur langsam booten. Docker-Container hingegen benötigen weniger Speicherplatz, da ihre Images normalerweise nur Dutzende von Megabytes groß sind. So können bei einem Einsatz von Docker mehr Anwendungen verarbeitet werden, was die Verwendung von VMs und Betriebssystemen reduziert. Auch ein Einsatz der Container auf Edge-Devices, z.B. auf kompakten Einplatinencomputern wie dem Raspberry Pi oder robusten und wartungsarmen Embedded PCs in der Industrie, ist problemlos möglich.
VM vs Docker

<img width="298" alt="Dock" src="https://user-images.githubusercontent.com/89446428/172340383-0f3b2362-2403-4e34-8d61-2ea65e7d42cb.PNG">

Docker-Container sind also flexibler und effektiver und die Verwendung von Docker in der Cloud ist sehr beliebt. Die Möglichkeit, dass verschiedene Anwendungen auf einer einzelnen Betriebssystem-Instanz ausgeführt werden können, verbessert vielfältige Einsatzmöglichkeiten immens. Ein entscheidender Vorteil von Docker-Containern ist die Fähigkeit, Apps nicht nur voneinander, sondern auch von ihrem zugrunde liegenden System zu isolieren. So kann der Anwender leicht bestimmen, wie eine zugewiesene containerisierte Einheit das jeweilige System und die vorhandenen Ressourcen (CPU, GPU und Netzwerk) nutzt. Zudem stellt es auch sicher, dass Daten und Code voneinander getrennt bleiben
