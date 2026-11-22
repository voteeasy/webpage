---
title: Als VoteEasy-Superadmin
subtitle: Wie VoteEasy selbst konfiguriert werden kann?
comments: false
---

Jede laufende VoteEasy-Anwendung verfügt über einen VoteEasy-Superadmin, der die laufende Instanz verwaltet und folgende Funktionen wahrnehmen kann:
* Organisationen manuell anlegen oder löschen
* Übersicht zur laufenden Instanz (Datenmenge)

Der Superadmin dient der Verwaltung Deiner laufenden VoteEasy-Anwendung und sollte - außer zu Testzwecken -
*nicht* zur regulären Abstimmungs-/Meetingarbeit verwendet werden!

Stattdessen kann man sich beliebig viele Organisationen anlegen und diese dann wieder löschen.

![Superadmin-Menü](/img/demo/superadmin/superadmin-menu.png)

# Organisationsverwaltung

Für jede Organisation lässt sich steuern, ob diese aktiv ist, sich also Nutzer anmelden können.

Auf diese Art und Weise kann man abbilden, dass man pro Meeting eine Organisation anlegt und diese nach deren Ende zu Archivierungszwecken deaktiviert, um die Daten zu konservieren.

Unter abgelaufenen Organisationen werden all jene Organisationen verstanden, die vor mehr als 60 Tagen angelegt wurden. So erkennt man noch einfacher, welche Organisationen vielleicht nicht mehr nötig sind und gelöscht werden können.

## Organisationseinstellungen

Daneben können pro Organisation spezifische Einstellungen (derzeit nur die Anzahl der generierbaren Zugangscodes) festgelegt werden.

![Org-Verwaltung](/img/demo/superadmin/organisationsverwaltung.png)

## Datenbankinhalte

Die Visualisierung der Datenbankinhalte zeigt, wie viele Organisationen, Nutzer, Zugangscodes und Abstimmungen in der laufenden VoteEasy-Instanz vorhanden sind. Es gibt diesen Menüpunkt einmal für die gesamte laufende Instanz und pro Organisation.

![ardinalitäten-graphisch](/img/demo/superadmin/datenbankinhalte-graphisch.png)

Pro Organisation ermöglicht die Anzeige eine Einschätzung zum Betrieb der Anwendung und zur Plausibilitätsprüfung (z.B. ob in der Organisation tatsächlich Abstimmungen vorhanden sind).

Dabei werden nur Anzahlen von Einträgen in Datenbanktabellen angezeigt (Kardinalitäten), keine Inhalte.

![Kardinalitäten-numerisch](/img/demo/superadmin/datenbankinhalte-zahlen.png)

## Versionsinformationen

Für Supportanfragen ist es nötig zu wissen, welcher Stand der VoteEasy-Instanz vorliegt. Diese Informationen sind im Menüpunkt "Versionsinformationen" abrufbar und beinhalten vorwiegend technische Parameter.

![Versionsinfo](/img/demo/superadmin/versionsinfo.png)

zurück zur [{{<icon class="fa fa-backward" style="font-size:16px;color:#ed9b57">}} Übersicht]({{< relref "/page/demo.md" >}})
