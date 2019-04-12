# Git - Eine (kurze) Einführung

In diesem Kapitel wird es darum gehen, wie du mit Git loslegen und die ersten Schritte tun kannst. 

## Was ist Git?

> Git [ɡɪt] ist eine freie Software zur verteilten Versionsverwaltung von Dateien, die durch Linus Torvalds initiiert wurde.  

[Wikipedia](https://de.wikipedia.org/wiki/Git)

Wie wir sehen werden, ist Git sehr mächtig und dennoch einfach zu lernen. 

## Was ist Versionsverwaltung? 

Bei einer Versionsverwaltung handelt e sich um ein System, welches die Änderungen an einer oder einer Reihe von Dateien über die Zeit hinweg protokolliert, sodass man später auf eine bestimmte Version zurückgreifen kann. 

Ein solches System erlaubt es, einzelne Dateien oder auch ein ganzes Projekt in einen früheren Zustand zurückzuversetzen, nachzuvollziehen, wer zuletzt welche Änderungen vorgenommen hat, die möglicherweise Probleme verursachen, herauszufinden wer eine Änderung ursprünglich vorgenommen hat und viele weitere Dinge. 

Ein Versionsverwaltungssystem bietet also die Möglichkeit, jederzeit zu einem vorherigen, funktionierenden Zustand zurückzukehren, wenn man einmal Mist gebaut oder aus irgendeinem Grunde Dateien verloren hat. 

### Distributed Version Control System (DVCS)

 Git ist eine sogenannt "Verteilte Versionsverwaltung". Bei verteilten Versionsverwaltungen erhalten die Anwender nicht einfach den letzten Snapshot des Projektes von einem Server, sondern eine **vollständige Kopie des gesamten Repositories**. 

![Bild 1](res/Bild_1.jpg)

Auf diese Weise kann, wenn ein Server beschädigt wird, jedes beliebige Repository von jedem beliebigen Anwenderrechner zurückkopiert werden und der Server so wiederhergestellt werden. Jede Kopie, ein sogenannter Klon (engl. clone), ist ein vollständiges Backup der gesamten Projektdaten.

## Die drei Zustände 

Die wichtigste Information, die man sich merken muss, wenn man Git erlernen und dabei Fallstricke vermeiden will ist, dass Git drei Hauptzustände kennt, in denen sich eine Datei befinden kann: 

1. **committed** - Die Daten sind sicher gespeichert in der lokalen Datenbank.  
2. **modified** - Die Daten wurden geändert, aber noch nicht in die lokale Datenbank gespeichert.
3. **staged** -  Geänderte (modified) Daten sind für den nächsten commit markiert.

## Die drei Hauptbereiche

Die drei Zustände führen uns direkt zu den drei Hauptbereichen eines Git Projektes: 

- das Git-Verzeichnis (Repository)
- das Arbeitsverzeichnis (Working Directory)
- die Staging-Area

![Bild 2](res/Bild_2.jpg)

### Git Directory

Das Git-Verzeichnis ist der Ort, an dem Git seine Metadaten und die lokale Datenbank für ein Projekt sichert. Dies ist der wichtigste Teil von Git. **In diesem Verzeichnis arbeitet Git und nur Git**, d.h. du lässt am besten die Finger davon und machst darin keine Änderungen. 

### Working Directory 

Das Arbeitsverzeichnis ist ein einzelnes Abbild einer spezifischen Version des Projektes. Die dort enthaltenen Dateien werden aus der komprimierten Datenbank geholt und auf der Festplatte in einer Form gespeichert, dass man sie nutzen und bearbeiten kann.

### Staging Area 

Die Staging Area ist einfach eine Datei, normalerweise befindet sich diese im Git-Verzeichnis, in der vorgemerkt wird, welche Änderungen der nächste Commit umfassen soll. Manchmal wird dieser Ort auch als "Index" bezeichnet, aber der Begriff Staging-Area ist der weiter verbreitet.

## Der Git-Workflow

Die grundlegenden Arbeitsschritte bei der Arbeit mit Git sind: 

![Bild 3](res/Bild_3.jpg)

## Werkzeuge 

Es gibt verschiedene Tools, welche die Arbeit mit Git unterstützen und ermöglichen. Auf der einen Seite gibt es die Kommandozeile, die **Git Bash** und auf der anderen Seite gibt es viele grafische Benutzeroberflächen, die sich im Leistungsumfang zum Teil beträchtlich unterscheiden. 

Wir werden ein einfaches Tool mit einer graphischen Benutzeroberfläche verwenden, und zwar **Git GUI**, welches bei der Installation von Git zusammen mit der Bash standardmässig installiert wird. 

