---
title: "Better Stundenplan vs Virtueller Stundenplan"
description: "Ein vergleich zwischen Better Stundenplan und Virtueller Stundenplan sowie deren offizieller app"
tags: ["Stundenplan", "Schule", "Vergleich", "Virtueller Stundenplan", "Virtueller Stundenplan App"]
showToc: false
draft: false
---

## Hinweis
Dieser Vergleich ist natürlich nicht objektiv. Falls du es noch nicht bemerkt hast, befindest du dich hier auf der Website von Better Stundenplan. 
Ich, als Entwickler dieser App, stehe natürlich meiner eigenen App positiver gegenüber und habe eine ✨ eher negative Meinung ✨ zu dem virtuellen Stundenplan ;)

Außerdem: Ich vergleiche nur die Benutzeroberflächen und deren Funktion, da alles auf dem Backend des virtuellen Stundenplans basiert.

## Der Vergleich

|  | ![](/images/icon.png) Better Stundenplan | ![](/images/comparison_vitrueller-stundenplan.png) Virtueller Stundenplan |  ![](/images/comparison_myBBS.png) myBBS (offizielle App) |
|--|--|--|--|
| Plattformen | Android¹ | Web | IOS, Android geplant |
| Bewertung | *N/A* | *N/A* | 2,8 von 5 Sternen² |
| Design | Material Design | *Keine Ahnung, auf jeden Fall scheiße* | Cupertino?³ |
| Datenquelle | Scraping der Website⁴ | *Ist die Website* | Offizielle API, hoffentlich⁵ |
| Tagesansicht | ✔ | ✔ | ✔ |
| Wochenansicht / Klassenplan | ✔ | ✔ | ?⁵ |
| Detailansicht | ✔ | ✗ | ✗ |
| Material You | ✔ | ✗ | ✗ |
| Aliasse | ✔ | ✗ | ✗ |
| Push-Benachrichtigungen | ✗ | ✗ | ✔ |
| Krankmelden | ✗ | ✔ | ✔ |
| Anwesenheiten | ✗ | ✔ | ✔ |
| Schülerausweis | ✗ | ✔ | ✔ |
| Lizenz | [MIT](https://github.com/LarvenStein/better-stundenplan/blob/main/LICENSE) | Proprietär | Proprietär |
| Preis | 0€ | 0€ | 0,99€ |
| Link | [Du bist schon hier :)](https://better-stundenplan.eike.in/) | ["Web-App"](https://virtueller-stundenplan.org/) | [AppStore](https://apps.apple.com/de/app/mybbs/id6449392034) |

---
## Fußnoten

1. Theoretisch ließe sich die App auch zu IOS, Windows, MAC, Linux und das Web compilen. Das mache ich aus folgenden Gründen nicht:
    * **IOS:** Zu teuer. 
    * **Windows, MAC, Linux:** Meiner Ansicht nach unnötig.
    * **Web-App:** [CORS](https://developer.mozilla.org/de/docs/Web/HTTP/CORS) macht die Sache unmöglich.
2. Aufgerufen am 03.03.2025 von [https://apps.apple.com/de/app/mybbs/id6449392034](https://apps.apple.com/de/app/mybbs/id6449392034)
3. Das "Apple-Design".
4. Die App tut so, als sei sie ein Besucher der Website des virtuellen Stundenplans. Die Daten holt sie sich aus der HTML-Struktur.
5. Ich weiß es hier nicht genau. Falls du es weißt, schreib mir unter [me@eike.in](mailto:me@eike.in)!