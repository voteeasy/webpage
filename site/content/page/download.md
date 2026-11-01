---
title: Downloads
subtitle: Anleitungen und der eigentliche Quellcode von VoteEasy. 
comments: false
---

# Anwendungsszenarien

VoteEasy kann Dir in vielen Anwendungsszenarien helfen:

{{< gallery caption-effect="fade" >}}
{{< figure thumb="-thumb" link="/img/wordcloud/wortwolke1-3-1024x1024.jpg" caption="Orte" alt="Anwendungsfälle 1/2" >}}
{{< figure thumb="-thumb" link="/img/wordcloud/wortwolke2-1-976x1024.jpg" caption="Anwendungsbeispiele" alt="Anwendungsfälle 2/2" >}}
{{< /gallery >}}

# Anleitungen

Da VoteEasy zwischen regulären Teilnehmern und Versammlungsleitern/Administratoren unterscheidet, hier eine Starthilfe:

* [{{<icon class="fa fa-file-pdf" style="font-size:32px;color:#ed9b57">}} Kurz-Leitfaden für Teilnehmer (PDF)](/pdf/download/easy_leitfaden_teilnehmer_1.3.pdf)
* [{{<icon class="fa fa-file-pdf" style="font-size:32px;color:#ed9b57">}} Step-By-Step-Handbuch für Teilnehmer (PDF)](/pdf/download/step_by_step_Teilnehmer_1.2.pdf)
* [{{<icon class="fa fa-file-pdf" style="font-size:32px;color:#ed9b57">}} Step-by-Step-Handbuch für Versammlungsleiter (PDF)](/pdf/download/step_by_step_Adminstrator_1.3.pdf)
* [{{<icon class="fa fa-image" style="font-size:32px;color:#ed9b57">}} VoteEasy-Logo für Deine Einladungen (PNG)](/img/download/voteeasy.png)

# Quellcode

Wir arbeiten intensiv an einer Freigabe via [{{<icon class="fab fa-github" style="font-size:32px;color:#ed9b57">}} GitHub](https://github.com/voteeasy).

Es existiert eine eigens dafür ins Leben gerufene GitHub-Organisation VoteEasy!

## Lizenz

VoteEasy wird unter der Lizenz [AGPL v3.0](https://www.gnu.org/licenses/agpl-3.0.de.html) zur Verfügung gestellt.

## Testsuite

Zur Absicherung gegen etwaige Regressionen, haben wir eine Testsuite entwickelt, die die wichtigsten Anwendungsfälle abdeckt.
Diese steht ebenfalls unter der Lizenz [AGPL v3.0](https://www.gnu.org/licenses/agpl-3.0.de.html) zur Verfügung und basiert technisch auf [Cypress](https://cypress.io).
Die Testsuite kann lokal ausgeführt werden, um die Funktionsfähigkeit der VoteEasy-Webanwendung zu prüfen.

[{{<icon class="fab fa-github" style="font-size:32px;color:#ed9b57">}} voteeasy/webapp-e2e-tests](https://github.com/voteeasy/webapp-e2e-tests)

## Webanwendung

Seit 2026-11-01 ist die erste Version der VoteEasy-Webanwendung verfügbar, die ebenso unter der Lizenz [AGPL v3.0](https://www.gnu.org/licenses/agpl-3.0.de.html) steht.

[{{<icon class="fab fa-github" style="font-size:32px;color:#ed9b57">}} voteeasy/webapp](https://github.com/voteeasy/webapp)

Die zugehörige Spring-Boot-Anwendung kann mit [Maven](https://maven.apache.org/) gebaut werden. Mittels [Docker](https://www.docker.com/) kann auch [PostgreSQL](https://www.postgresql.org/) als Datenbank verwendet werden.

## Webseite selbst

Diese Webseite selbst ist ebenfalls Open Source und kann unter [{{<icon class="fab fa-github" style="font-size:32px;color:#ed9b57">}} voteeasy/webpage](https://github.com/voteeasy/webpage) gefunden werden.
Als technische Infrastruktur wird [Hugo](https://gohugo.io/) verwendet, um die eigentliche statische Webseite zu generieren.
Das verwendete Theme lautet Beautiful Hugo und ist unter [{{<icon class="fab fa-github" style="font-size:32px;color:#ed9b57">}} beautifulhugo](https://github.com/halogenica/beautifulhugo) verfügbar.
