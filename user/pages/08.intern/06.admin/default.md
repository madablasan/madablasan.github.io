---
title: Admin-Bereich
visible: false
taxonomy:
  tag: intern
---

# Administrator-Bereich

Auf dieser Seite findest du Informationen dazu, wie du die Inhalte dieser [CCB-Homepage](http://www.charitechorberlin.de?target=_parent) bearbeiten kannst.<br />
Solltest du kein CCB-Homepage-Administrator sein, ist diese Anleitung für dich völlig irrelevant. Falls du sie trotzdem durchlesen möchtest, wird dich allerdings niemand dran hindern - denn du kennst das wichtige Login-Passwort sowieso nicht <img src="http://www.madtv-online.com/madtv/forum/images/smilies/standart/wink.gif" />.

**Wichtig für Admins:** Bitte ändert nichts an dieser Anleitungs-Seite und löscht sie auch nicht!

## Seiteninhalte bearbeiten

1. Logge dich beim [Lima-City File Manager](https://filemanager.lima-city.de?target=_blank) ein mit dem Benutzernamen _charite-chor-berlin_ und dem File-Manager-Passwort.
2. Du siehst ein Fenster mit Datei- und Ordner-Informationen. Klicke nacheinander auf die Ordnernamen _charite-chor-berlin.lima-city.de_, _user_ und _pages_.

**Wichtig:** Sobald du eingeloggt bist, nutze bitte _nicht_ den "Seite-zurück"-Pfeil deines Browsers, sonst wirst du wieder ausgeloggt! Wenn du aus einem Verzeichnis zurückspringen möchtest, klicke bitte auf den Text _Aufwärts_ mit dem Ordnersymbol daneben. 

Jedes **Menü**, das es auf der CCB-Homepage gibt, hat einen eigenen Ordner. Die **Zahl vor dem Ordnernamen** gibt die **Reihenfolge** der Menüs an. Wenn du z. B. die Ordner "01.home" und "02.ueber_uns" umbenennst in "01.ueber_uns" und "02.home", dann rutscht das Home-Menü einen Platz weiter nach links.

Der **Seiteninhalt** eines Menüs ist im jeweiligen Menü-Ordner unter dem Dateinamen "default.md" gespeichert. Wenn du z. B. auf den Ordner "01.home" klickst, siehst du eine "default.md"-Datei, welche den Inhalt der Startseite enthält.
 
Um eine "default.md"-Datei zu bearbeiten, klicke rechts unter **Aktionen** auf **Bearbeiten**. Es öffnet sich ein Textfeld, in welchem du den Inhalt der Seite bearbeiten kannst. Der obere Bereich zwischen den drei Strichen (---) sollte nur von Personen verändert werden, die Erfahrung mit dem _Grav_-Framework haben. Falls du dich wunderst, warum manche Worte mit Sternchen, Unterstrichen oder Rautezeichen (#) geschmückt sind: Das ist die so genannte _MarkDown-Syntax_ (siehe unterer Abschnitt).

Einige Menü-Ordner enthalten **Untermenüs**. Das sieht man daran, dass es neben der "default.md"-Datei auch weitere Ordner gibt. Die Zahlen vor den Untermenü-Ordnern geben die (vertikale) Reihenfolge an, in der die Untermenüs angezeigt werden. Öffne z. B. den Ordner "02.ueber_uns", dort siehst du 2 Ordner "01.das_sind_wir" und "02.unsere_projekte". Wenn du sie umbenennst in "01.unsere_projekte" und "02.das_sind_wir", erscheinen die Untermenüs in umgekehrter Reihenfolge.

Jeder Untermenü-Ordner enthält wiederum eine "default.md"-Datei mit dem Seiteninhalt des Untermenüs.

## Die _MarkDown-Syntax_

Damit die einzelnen Seiten der CCB-Homepage nicht so langweilig aussehen, kann man Texte fett, kursiv und unterstrichen darstellen sowie Links, Bilder und Tabellen einbauen.

**Überschriften**: Es gibt sechs Typen von Überschriften (von denen aber normalerweise maximal drei genutzt werden sollten). Die Haupt-Überschrift startet mit einem Rautezeichen (#) vor dem Text, die nächst untergeordnete Überschrift mit zwei Rautezeichen, die dritte mit drei Rautezeichen usw.

**Fett, kursiv, unterstrichen usw.:** Um Text fett zu drucken, muss er mit zwei Sternchen-Symbolen umgeben werden (&#42;&#42;Ich bin fett&#42;&#42; wird zu **Ich bin fett**). Kursiver Text wird mit Unterstrichen umgeben (&#95;Ich bin kursiv&#95; wird zu _Ich bin kursiv_). Text, der unterstrichen werden soll, muss etwas umständlich formatiert werden: &lt;u&gt;Ich bin unterstrichen&lt;/u&gt; wird zu <u>Ich bin unterstrichen</u>. Wenn ein Text durchgestrichen werden soll, wird er mit zwei Tilde-Symbolen (~) umgeben: &#126;&#126;Ich bin durchgestrichen&#126;&#126; wird zu ~~Ich bin durchgestrichen~~. Diese Kürzel können miteinander kombiniert werden, z.B. &#42;&#42;&#95;Ich bin fett und kursiv&#95;&#42;&#42; wird zu **_Ich bin fett und kursiv_** oder &#126;&#126;&lt;u&gt;Ich bin unterstrichen und durchgestrichen&lt;/u&gt;&#126;&#126; wird zu ~~<u>Ich bin unterstrichen und durchgestrichen</u>~~.
 
**Links einfügen:** Ein Link besteht aus zwei Teilen, der URL-Adresse (so etwas wie _http://www.charitechorberlin.de_) und dem Text, der über dem Link angezeigt werden soll. Der Link-Text wird in eckige Klammern gesetzt, gefolgt von der URL-Adresse, welche in runde Klammern gesetzt wird. Beispiel: &#91;Startseite vom Charité Chor&#93;&#40;http://www.charitechorberlin.de&#41; wird zu [Startseite vom Charité Chor](http://www.charitechorberlin.de?target=_parent).<br />
**Ganz wichtig:** Immer wenn du einen Link setzen willst, der auf eine der CCB-Seiten verweist (z. B. ein Verweis auf unsere Konzertübersicht), musst du hinter der URL-Adresse des Links folgendes schreiben: **?target=_parent**. Also z.B. &#91;Konzertübersicht&#93;&#40;http://charitechorberlin.de/konzerte?target=_parent&#41; wird zu [Konzertübersicht](http://charitechorberlin.de/konzerte?target=_parent). Frag nicht warum das so sein muss, kopier' es einfach in jeden internen Link <img src="http://www.madtv-online.com/madtv/forum/images/smilies/standart/wink.gif" />. Und falls du möchtest, dass ein Link in einem neuen Browser-Tab geöffnet wird, schreibst du stattdessen: **?target=_blank**.

**Bilder einfügen**: Die Syntax beim Bilder einfügen sieht so ähnlich aus wie bei den Links. Du musst den Bildpfad kennen, welcher eine URL-Adresse ist <!--(siehe auch Abschnitt **Medien-Dateien verwalten**)-->. Dann wird das Bild mit folgender Syntax eingebaut: &#33;&#91;&#93;&#40;http://url-adresse-des-bildes&#41; (ein Ausrufezeichen, eine öffnende und schließende Klammer direkt nacheinander und dann in runden Klammern die Bild-URL-Adresse). Wenn z. B. das CCB-Logo angezeigt werden soll, macht man das mit &#33;&#91;&#93;&#40;http://charite-chor-berlin.lima-city.de/user/pages/images/CCB-Logo.png&#41;:<br /> ![](http://charite-chor-berlin.lima-city.de/user/pages/images/CCB-Logo.png?classes=thumbnail)<br />
**Wichtig:** Die von den CCB-Homepage-Admins selbst hochgeladenen Bilder sollten in der Regel unter der URL-Adresse http://charite-chor-berlin.lima-city.de/user/pages/images/<i>Name-der-Bilddatei</i> zu finden sein.<br />
**Auch wichtig:** Damit die Bilder nicht immer riesig auf dem Bildschirm dargestellt werden, gibt es mehrere "Style-Klassen", um die Größe und Ausrichtung anzupassen. Eine Style-Klasse wird dem Bild mit dem Parameter <i>?classes=name-der-styleklasse</i> angegeben (z. B. &#33;&#91;&#93;&#40;http://charite-chor-berlin.lima-city.de/user/pages/images/CCB-Logo.png?classes=img-small&#41;). Folgende Klassennamen gibt es: _img_ (für große Bilder unter Überschriften), _img-medium_ (für mittelgroße Bilder unter Überschriften, wie z. B. bei Chorleiter und Stimmbildner), _img-small_ (für kleine Bilder im Fließtext) und _thumbnail_ (für Vorschaubilder, die nicht zentriert sondern linksbündig ausgerichtet werden).

**Tabellen einfügen:** Eine Tabelle braucht immer eine Kopfzeile, wo die einzelnen Tabellenspalten beschrieben werden. Spalten werden durch Senkrechtstriche ( | ) voneinander getrennt, und unter die Kopfzeile schreibt man eine gestrichelte Linie aus Minuszeichen. Hier ein Beispiel:

Name&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&#124; Adresse&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&#124; Telefonnummer<br />
----------------&#124;-------------------------------------&#124;--------------<br />
Max Mustermann  &#124; Musterstraße 123, 0815 Musterhausen &#124; 12345678<br />
Fritzchen Frech &#124; Alberner Weg 12, 66666 Bösestadt    &#124; 45798023

wird zu 

Name            | Adresse                             | Telefonnummer
----------------|-------------------------------------|--------------------
Max Mustermann  | Musterstraße 123, 0815 Musterhausen | 12345678
Fritzchen Frech | Alberner Weg 12, 66666 Bösestadt    | 45798023

## Technische Details

Die Domain www.charitechorberlin.de ist auf dem kostenlosen Webspace lima-city.de abgelegt. Das Username ist charite-chor-berlin. Das Passwort ist Marco und dem Vorstand bekannt.
<!--
Die Domain "http://www.charitechorberlin.de" ist auf irgendeinem Webspace abgelegt. Es ist lediglich der Provider bekannt ([Uberspace](https://uberspace.de?target=_blank)), aber es gibt keine öffentlich bekannten Zugangsdaten, um auf den eigentlichen Inhalt der CCB-Homepage direkt zuzugreifen. Der Direktzugriff ist nur zwei Personen möglich, Dominik Weis (Administrator, [Email schicken](mailto:d.weis@fu-berlin.de)) und Stefan Behrendt (User mit eingeschränkten Rechten, [Email schicken](mailto:stefankjbehrendt@aol.com)).

Um diesen unschönen Zustand etwas zu verbessern, wurde der CCB-Homepage-Inhalt auf einen kostenfreien Webspace vom Anbieter [Lima-City](https://www.lima-city.de?target=_blank) kopiert. Die CCB-Homepage enthält nur ein einziges **IFrame**-Element, welches den Seiteninhalt von der Lima-City-Kopie lädt und anzeigt. Damit Links nicht innerhalb des IFrame-Fensters, sondern im übergeordneten CCB-Homepage-Fenster geladen werden, muss bei jedem Link das Attribut **target="_parent"** gesetzt werden!

Sollte der Inhaber des Domain-Webspaces von "http://www.charitechorberlin.de" (Dominik Weis) den Webspace irgendwann kündigen und die CCB-Homepage wäre unter "http://www.charitechorberlin.de" nicht mehr erreichbar, dann kann man sie trotzdem immer noch unter "charite-chor-berlin.lima-city.de" abrufen. -->