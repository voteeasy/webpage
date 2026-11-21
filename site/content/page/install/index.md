---
title: Installation
subtitle: Wie bringe ich VoteEasy für mich zum Laufen?
comments: false
---

## Technologiestack

Als Administrator sollte man sich mit den folgenden Technologien auskennen, um VoteEasy installieren und betreiben zu können:

* Programmiersprache: [Java](https://java.sun.com) 17
* Framework: [SpringBoot](https://spring.io/projects/spring-boot) Version 3
* Datenbank: [PostgreSQL](https://www.postgresql.org/) (andere sind aber möglich und konfigurierbar)
* Frontend: HTML5, CSS3, JavaScript, Bootstrap 5.3.2
* Build-Tool: [Maven](https://maven.apache.org/)
* Containerisierung: [Docker](https://www.docker.com/)

## Lizenzbedingungen

Die Anwendung selbst ist unter der Lizenz [AGPL v3.0](https://www.gnu.org/licenses/agpl-3.0.de.html) verfügbar und kann lokal installiert werden. Änderungen am Quellcode sind möglich und können in der eigenen Installation vorgenommen werden. Weiterentwicklung und umfangreichere Anpassungen sind möglich, solange die Lizenzbedingungen eingehalten werden.

## Installationshinweise

### {{<icon class="fa fa-people-group" style="font-size:32px;color:#ed9b57">}} Zugangsdaten

Standardmäßig gibt es in VoteEasy **drei** Organisationen, die mit Beispieldaten gefüllt sind. Die Zugangsdaten sind:

* VoteEasy-Organisation: `voteeasy`
* VoteEasy-Administrator: `gongbing`
* VoteEasy-Administrator-Passwort: `gongbing`

### {{<icon class="fa fa-magnifying-glass-plus" style="font-size:32px;color:#ed9b57">}} Installation für Ungeduldige

Unter der Annahme, dass Java, Maven und Docker bereits installiert sind, kann VoteEasy mit den folgenden Befehlen gestartet werden:

```bash
git clone https://github.com/voteeasy/webapp.git
cd webapp
./sh/cleanUpDBAndStartDocker.sh
```

Die Anwendung ist dann in der Standardkonfiguration unter [http://localhost:8080](http://localhost:8080) aufrufbar.

## Individuelle Unterstützung und Anfragen

VoteEasy ist ein einfaches Abstimmungstool, das als freie Software zur Verfügung steht.

Bei technischen oder inhaltlichen Anfragen besteht die Möglichkeit, sich [individuell zu melden](&#109;&#97;&#105;&#108;&#116;&#111;&#58;&#118;&#111;&#116;&#101;&#101;&#97;&#115;&#121;&#64;&#97;&#105;&#107;&#105;&#45;&#105;&#116;&#46;&#100;&#101;&#63;&#115;&#117;&#98;&#106;&#101;&#99;&#116;&#61;&#65;&#110;&#102;&#114;&#97;&#103;&#101;&nbsp;&#122;&#117;&nbsp;&#86;&#111;&#116;&#101;&#69;&#97;&#115;&#121;).
Ein kostenpflichtiger Support ist vereinbar und grundsätzlich möglich.

Wir finden einen Weg.

