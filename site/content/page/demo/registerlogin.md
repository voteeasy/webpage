---
title: Login & Registrierung
subtitle: Wie startet man mit VoteEasy?
comments: false
---

# Selbstregistrierung

Um mit VoteEasy zu starten, muss man zuerst für sich eine eigene Organisation, auch Tenant genannt, registrieren.
Dies kann man selbst tun:

![Registrierung - Name](/img/demo/registerlogin/selbstregistrierung-start.png)

Beispielsweise kann eine Organisation registriert werden, die **test** heißt. 

In dieser werden nach erfolgter Selbstregistrierung zwei Nutzer (Administrator und regulärer Teilnehmer) angelegt.
Ebenso werden Beispieldaten in der Organisation erzeugt, die zeigen, wie man VoteEasy verwenden kann.

Diese können vom Administrator der Organisation entfernt werden.

![Registrierung - Erfolg](/img/demo/registerlogin/selbstregistrierung-erfolg.png)

Nach erfolgter Selbstregistrierung einer Organisation werden die initialen Zugangsdaten angezeigt.
Diese müssen notiert werden, da sie nur durch Löschen und Neuanlage wieder erzeugt werden können vom VoteEasy-Superadmin.

Ein Login ist sofort nach Registrierung per QR-Code oder direkter Eingabe im Webformular möglich!

# Login

Solange man nicht bei VoteEasy angemeldet ist, kann man die Anwendung nicht verwenden.

![Login](/img/demo/registerlogin/login.png)

Nach erfolgter Selbstregistrierung - dem obigen Beispiel folgend - würde man in die drei Formularfelder die Werte
* **test** = Ihre Organisation
* **test-admin** = Ihr Benutzername
* **mqoXsj** = Ihr Passwort

eintragen und sich anmelden können.

## mit Zugangscode

Hat man vom Organisationsadmin einen Zugangscode erhalten, so muss man diesen als Benutzername eingeben, um den Token einmalig zu aktivieren und Zugang zu VoteEasy zu erhalten.

Im Beispiel wäre hier **00961102-87** der einzugebende Benutzername, um sich mit einem selbst gewählten Passwort kombiniert zu registrieren und anzumelden.

![Token](/img/demo/registerlogin/tokenbeispiel.png)

Nachdem der Zugangscode einmal verwendet wurde, kann er nicht mehr zur Registrierung verwendet werden.
Stattdessen kann man sich mit dem Code als Nutzername regulär anmelden.

# Anmeldung

## als Teilnehmer

Als regulärer Teilnehmer sieht man im Seitenfuß einen grünen Kringel.
Man kann nur an Abstimmungen teilnehmen.

## als Administrator

Als Administrator einer Organisation sieht man im Seitenfuß einen grünen und einen gelben Kringel und hat ein orange gefärbtes Admin-Menü in der Menüleiste.
Neben der Teilnahme an Abstimmungen kann der Administrator neue Abstimmungen konfigurieren und selbst an Abstimmungen teilnehmen.

## als VoteEasy-Superadmin

Als Superadmin sieht man im Seitenfuß einen grünen, gelben und roten Kringel und hat ein rot gefärbtes Admin-Menü in der Menüleiste.

**<i class="fa fa-warning" style='font-size:16px;color:#ed9b57'></i> Dieser Nutzer sollte nicht für Abstimmungen o.ä. benutzt werden, da er vorwiegend administrative Aufgaben wahrnimmt.**

zurück zur [<i class="fa fa-backward" style='font-size:16px;color:#ed9b57'></i> Übersicht]({{< relref "/page/demo.md" >}})
