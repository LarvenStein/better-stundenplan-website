---
title: "FAQ zu Better Stundenplan"
description: "Hier beantworte ich häufig gestellte fragen zu Better Stundenplan"
tags: ["Virtueller Stundenplan", "Virtuelles Klassenbuch", "Virtueller Stundenplan App"]
showToc: true
draft: false
date: 2025-03-13
---

## Wie werden meine Login-Daten gespeichert?
Deine Login-Daten werden mittels `SharedPreferences` **unverschlüsselt** auf deinem Handy gespeichert. Ich empfehle, das dort verwendete Passwort nirgendwo anders zu verwenden.

## Warum sind alle Fächer (Farbe)?
Die App verwendet, sofern verfügbar, die Material You Farben deines Handys, ansonsten ein Farbschema aus einem Orangeton. Fächer verwenden aktuell die Primärfarbe dieses Farbschemas. Automatisch werde ich keine verschiedenen Farben für verschiedene Fächer anzeigen, da dies emotionale Reaktionen bei Verwender*innen hervorruft. Zukünftig könnte ich ermöglichen, Farben für Fächer festzulegen. Dazu habe ich aber aktuell keine Lust.

## iOS App
Eine iOS-App ließe sich theoretisch aus meinem Code kompilieren, davon sehe ich aktuell aber ab, da das Veröffentlichen für iOS entweder einiges an Geld oder eine komplizierte Sideloading-Prozedur erfordert.
Du kannst gerne versuchen, die App für dein iPhone zu kompilieren, [melde dich mit Ergebnissen gerne bei mir](mailto:me@eike.in) :)

## Woher kommen die Daten?
An die Daten des Stundenplans komme ich, indem die App normale Anfragen an die Website des Stundenplans wie ein normaler Besucher sendet und aus dem HTML dann benötigte Daten extrahiert.

## Warum machst du das?
Diese App ist im Rahmen eines Schulprojektes entstanden. Selbst finde ich den virtuellen Stundenplan schrecklich, weshalb ich ein alternatives Frontend gebaut habe. Mehr Unterschiede findest du [in diesem Post](https://better-stundenplan.eike.in/posts/better-stundenplan-vs-mybbs/).

## Wie installiere ich das?
Da ich aktuell zu faul bin, die App in Stores zu veröffentlichen, musst du die App mittels einer APK installieren. Lade diese aus [dem neusten GitHub Release](https://github.com/LarvenStein/better-stundenplan/releases) auf deinem Android-Handy [herunter](https://github.com/LarvenStein/better-stundenplan/releases) und öffne diese Datei. Durch den Rest leitet dich dein Handy durch.
[![](/images/apk-badge.png)](https://github.com/LarvenStein/better-stundenplan/releases)

## Ist die App kostenlos?
Die App ist komplett kostenlos und Open Source. Der gesamte Quellcode ist auf GitHub verfügbar.

## Werden meine Daten an Dritte weitergegeben?
Nein, deine Daten werden ausschließlich für die Kommunikation mit dem Stundenplan-Server verwendet und nicht an Dritte weitergegeben.

## Kann ich bei der Entwicklung helfen?
Ja, die App ist Open Source und ich freue mich über Beiträge. Du kannst auf GitHub Issues erstellen oder Pull Requests einreichen.

## Welche Berechtigungen benötigt die App?
Die App benötigt nur Internetzugriff, um die Stundenplan-Daten abzurufen. Es werden keine weiteren Berechtigungen benötigt.

## Was passiert, wenn der offizielle Stundenplan geändert wird?
Da die App direkt mit der offiziellen Website kommuniziert, kann es bei größeren Änderungen zu Kompatibilitätsproblemen kommen. In diesem Fall werde ich versuchen, zeitnah ein Update bereitzustellen.
