---
title: "Virtueller Stundenplan: Eine Gefahr für Sicherheit und Nerven"
description: "Peinliche Sicherheitslücken und Dinge, die man einfach nicht macht"
tags: ["Virtueller Stundenplan", "Virtuelles Klassenbuch"]
showToc: false
draft: false
date: 2025-03-07
---

Hier möchte ich darüber sprechen, warum ich denke, dass das Entwicklungsteam des Virtuellen Stundenplans inkompetent ist und einen Einsatz dieser Software für gefährlich halte.

> **Disclaimer:** 
> Dies ist kein journalistischer Artikel, sondern ein persönlicher Kommentar eines ✨leicht genervten✨ Anwenders dieser Software. Die hier geäußerten Meinungen basieren auf meinen eigenen Erfahrungen mit dem Virtuellen Stundenplan.

## Grundlegende Probleme

Der "Virtuelle Stundenplan" präsentiert sich mit einem katastrophalen Benutzerinterface, das von ständigen Fehlern und Ausfällen geplagt wird. In meinem Fall ist mein Profil einfach mal verschwunden. In der Anwesenheit war es weg und einloggen konnte ich mich auch nicht mehr. Irgendwann ist es wie durch ein Wunder wieder aufgetaucht.

Bei der Nutzung der Plattform tauchen regelmäßig SQL-Fehler auf der Startseite auf – ein deutliches Zeichen für mangelhafte Programmierung und fehlende Qualitätskontrolle. 
![SQL Fehler auf der Startseite des virtuellen Stundenplans.](/images/virtueller-stundenplan-ein-disaster/sql-error.png) *Ein SQL Fehler auf der Startseite. `snr` steht für eine Schulnummer, nehme ich an.*

Das HTML ist kaputt und grauenhaft formatiert, mit mehreren schließenden `<body>`-Tags und zahlreichen unnötigen Kommentaren im Code.
![Die Zumutung einer HTML-Struktur](/images/virtueller-stundenplan-ein-disaster/html.png) *Unleserlich, aber nicht minifiziert und mehrere schließende Body-tags. Klasse!*

## Unlogische Struktur

Die Benennung der Seiten folgt keinerlei erkennbarer Logik: Der 1-Tages-Plan ist unter `/page2/` und Tabellen-Symbol einem zu finden, während der Wochenplan unter `/page-5/` und einem "mehrere-personen"-Symbol versteckt ist. Wo ist hier der Sinn? Eine intuitive Navigation sucht man vergebens.

## Peinliche Sicherheitsprobleme

Besonders alarmierend sind jedoch die peinlichen Sicherheitsprobleme und die inkompetenten Lösungsversuche des Entwicklungsteams:

In die Klassenauswahl auf `page-5` lässt sich HTML injizieren, welches auf der Seite gerendert wird. Dadurch konnte ich eine Cross-Site-Scripting-Attacke durchführen, die potenziell Login-Daten von Nutzern abgreifen **könnte**.

![Ein Beispiel für Cross-Site-Scripting auf dem Stundenplan](/images/virtueller-stundenplan-ein-disaster/cross-site-scripting.png) *Sollte ich das zeigen? Ups 🥸*

Eine direkte Kontaktmöglichkeit für Sicherheitsmeldungen existiert nicht – ich musste den Umweg über den Schulleiter nehmen, um das Problem zu melden. Die "Lösung" des Teams bestand lediglich darin, bestimmte Tags wie `<form>` oder `<script>` aus dem injizierten HTML zu entfernen.

Das eigentliche Problem bleibt jedoch bestehen: Ich kann **immer noch** JavaScript durch `<img src="" onerror" /* JavaScript /*">` ausführen – eine Methode, die ich sogar in meiner ursprünglichen Meldung erwähnt hatte!

Am 26. September 2024 habe ich dieses Problem erneut gemeldet und dabei sogar auf eine PHP-Methode hingewiesen, die das Problem beheben würde. Seitdem habe ich nichts mehr gehört. Das Problem besteht weiterhin.

## Fazit

Die Kombination aus schlechtem Design, fehlerhafter Implementierung und peinlichen Sicherheitslücken macht den "Virtuellen Stundenplan" zu einer, meiner Meinung nach, gefährlichen Software, deren Einsatz in Bildungseinrichtungen dringend überdacht werden sollte.