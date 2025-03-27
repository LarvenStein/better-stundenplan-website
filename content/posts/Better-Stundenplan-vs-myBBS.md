---
title: "Better Stundenplan vs Virtueller Stundenplan"
description: "Ein Vergleich zwischen Better Stundenplan und Virtueller Stundenplan sowie deren offizieller App"
tags: ["Stundenplan", "Schule", "Vergleich", "Virtueller Stundenplan", "Virtueller Stundenplan App"]
showToc: false
draft: false
date: 2025-03-06
lastmod: 2025-03-27
---

> **Update 27.03.2025:**
> Es wurde eine Android-Version von myBBS veröffentlicht. Den Vergleich habe ich angepasst.

## Hinweis
Dieser Vergleich ist natürlich nicht objektiv. Falls du es noch nicht bemerkt hast, befindest du dich hier auf der Website von Better Stundenplan. 
Ich, als Entwickler dieser App, stehe natürlich meiner eigenen App positiver gegenüber und habe eine ✨ eher negative Meinung ✨ zu dem virtuellen Stundenplan ;)

Außerdem: Ich vergleiche nur die Benutzeroberflächen und deren Funktion, da alles auf dem Backend des virtuellen Stundenplans basiert.

## Der Vergleich
<div>
    <table>
        <thead>
            <tr>
                <th></th>
                <th>
                    <img src="/images/icon.png">
                    Better Stundenplan
                </th>
                <th>
                    <img src="/images/comparison_vitrueller-stundenplan.png">
                    Virtueller Stundenplan
                </th>
                <th colspan="2">
                    <img src="/images/comparison_myBBS.png">
                    myBBS (offizielle App)
                </th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Plattformen</td>
                <td>Android¹</td>
                <td>Web</td>
                <td>iOS</td>
                <td>Android</td>
            </tr>
            <tr>
                <td>Bewertung</td>
                <td><em>N/A</em></td>
                <td><em>N/A</em></td>
                <td>2,8 von 5 Sternen²</td>
                <td><em>N/A</em></td>
            </tr>
            <tr>
                <td>Design</td>
                <td>Material Design</td>
                <td><em>Keine Ahnung, auf jeden Fall scheiße</em></td>
                <td>Cupertino?³</td>
                <td>Schlechtes Material Design⁶</td>
            </tr>
            <tr>
                <td>Datenquelle</td>
                <td>Scraping der Website⁴</td>
                <td><em>Ist die Website</em></td>
                <td>Offizielle API, hoffentlich⁵</td>
                <td>Offizielle API, wahrscheinlich</td>
            </tr>
            <tr>
                <td>Tagesansicht</td>
                <td>✔</td>
                <td>✔</td>
                <td>✔</td>
                <td>✔</td>
            </tr>
            <tr>
                <td>Wochenansicht / Klassenplan</td>
                <td>✔</td>
                <td>✔</td>
                <td>?⁵</td>
                <td>✗</td>
            </tr>
            <tr>
                <td>Detailansicht</td>
                <td>✔</td>
                <td>✗</td>
                <td>✗</td>
                <td>✗</td>
            </tr>
            <tr>
                <td>Material You</td>
                <td>✔</td>
                <td>✗</td>
                <td>✗</td>
                <td>Nur einzelne Farben⁶</td>
            </tr>
            <tr>
                <td>Aliasse</td>
                <td>✔</td>
                <td>✗</td>
                <td>✗</td>
                <td>✗</td>
            </tr>
            <tr>
                <td>Push-Benachrichtigungen</td>
                <td>✗</td>
                <td>✗</td>
                <td>(✔)⁷</td>
                <td>(✔)⁷</td>
            </tr>
            <tr>
                <td>Krankmelden</td>
                <td>✗</td>
                <td>✔</td>
                <td>✔</td>
                <td>✔</td>
            </tr>
            <tr>
                <td>Anwesenheiten</td>
                <td>✗</td>
                <td>✔</td>
                <td>(✔)⁷</td>
                <td>(✔)⁷</td>
            </tr>
            <tr>
                <td>Schülerausweis</td>
                <td>✗</td>
                <td>✔</td>
                <td>✔</td>
                <td>✔</td>
            </tr>
            <tr>
                <td>Lizenz</td>
                <td><a href="https://github.com/LarvenStein/better-stundenplan/blob/main/LICENSE">MIT</a></td>
                <td>Proprietär</td>
                <td>Proprietär</td>
                <td>Proprietär</td>
            </tr>
            <tr>
                <td>Preis</td>
                <td>0€</td>
                <td>0€</td>
                <td>0,99€</td>
                <td>0,99€</td>
            </tr>
            <tr>
                <td>Link</td>
                <td><a href="https://better-stundenplan.eike.in/">Du bist schon hier :)</a></td>
                <td><a href="https://virtueller-stundenplan.org/">"Web-App"</a></td>
                <td><a href="https://apps.apple.com/de/app/mybbs/id6449392034">AppStore</a></td>
                <td><a href="https://play.google.com/store/apps/details?id=de.bbs_verwaltung.myBBS">PlayStore</a></td>
            </tr>
        </tbody>
    </table>
</div>

---
## Fußnoten

1. Theoretisch ließe sich die App auch zu iOS, Windows, Mac, Linux und das Web compilen. Das mache ich aus folgenden Gründen nicht:
    * **iOS:** Zu teuer. 
    * **Windows, Mac, Linux:** Meiner Ansicht nach unnötig.
    * **Web-App:** [CORS](https://developer.mozilla.org/de/docs/Web/HTTP/CORS) macht die Sache unmöglich.
2. Aufgerufen am 03.03.2025 von [https://apps.apple.com/de/app/mybbs/id6449392034](https://apps.apple.com/de/app/mybbs/id6449392034)
3. Das "Apple-Design".
4. Die App tut so, als sei sie ein Besucher der Website des virtuellen Stundenplans. Die Daten holt sie sich aus der HTML-Struktur.
5. Ich weiß es hier nicht genau. Falls du mehr weißt, schreib mir unter [me@eike.in](mailto:me@eike.in)!
6. Die App basiert zwar auf Material Design, es werden aber beispielsweise nur einzelne Farben aus dem System geholt. Dadurch ist, falls das Smartphone im Dark-Mode ist, beim Stundenplan der Hintergrund sowie die Schriftfarbe weiß, was die App unbrauchbar macht. (Stand 27.03.2025)
7. Hängt scheinbar von der Schule ab. An der BBS Papenburg und mit der Android-App (v1.0) ging es nicht. (Stand 27.03.2025)