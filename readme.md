#Inhalt der KAZOOSH-Webseite

Die Ordnerstruktur ist folgendermaßen aufgebaut:

```
|- content [Markdown Dateien]
	|- root
		|- mitglieder
		|- news
		|- projekte
		|- workshops
|- images [Bilder zu den Artikeln]
	|- home
	|- kontakt
	|- mitglieder
		|- vorname_nachname1
		|- vorname_nachname2
		|- vorname_nachname3
		...
	|- projekte
		|- 20xx_projektname1
		|- 20xx_projektname2
		|- 20xx_projektname3
		...
	|- workshops 
		|- 20xx_projektname1
		|- 20xx_projektname2
		|- 20xx_projektname3
		...
```

## Editieren von Artikeln

Sämtlich Texte befinden sich in /content und sind als markdown Dateien verfasst. Diese Inhalte werden für die Webseite konvertiert. 

Aufbau einer Markdown-Datei:

```
---
title: hier sind metadaten

---

Hier kommt der Text. Der Text kann formatiert werden:

### Überschrift

#### Unter-Überschrift

Text
```

Die Bilder befinden sich meist im korrespondierenden /images Ordner des jeweiligen Artikels

Beispielprojekt:

```
/content/projekte/2011_beispielprojekt.md [das Beispielprojekt]
/images/projekte/2011_beispielprojekt/123.jpg [beispielbild]
```

## Beispiele für Artikel

Für verschiedene Artikel gibt es verschiedene Metadaten.

### Menüseiten (Kontakt, Projekte ...)

```
---
order: 4 [Reihenfolge in Navigation]
title: Kontakt [Titel]

images:
- kontakt/header.jpg [Headerbild]

---

[Beschreibungstext in weißer Box]
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. 
```

### Mitgliederseiten
```
---
title: Thorben Friedrich [name]
images: [Reihenfolge ist wichtig]
- mitglieder/thorben_friedrich/profil.jpg [Profilbild]
- mitglieder/thorben_friedrich/banner.jpg [Banner-Bild]


lastname: Friedrich
firstname: Thorben
profession: Medieninformatiker

email: thorben@kazoosh.com
homepage: http://thorben.com
github: https://github.com/thorben
vimeo: https://vimeo.com/user123456

interests: [beliebig viele können aufgelistet werden]
- Arduino
- Programmierung
- Konzeption

---
[Beschreibungstext]
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, 
```

###Projektseiten, Workshopseiten 
```
---
title: Heat [Name des Projekts]
teaser: [Der Vorschautext]

images: [mindestens 3 Bilder sind notwendig]
- projekte/2013_heat/heat.png [Banner-Bild]
- projekte/2013_heat/heat02.jpg [Artikelbild 1]
- projekte/2013_heat/heat03.jpg [Artikelbild 2]
- projekte/2013_heat/heat...    [beliebig viele weitere Bilder in Galerie]

video: http://player.vimeo.com/video/101627787 [Vimeo-Video-Link]

date: 2013 [Jahr]
location: Festspielhaus Hellerau [Ort]

festival: CYNETART [Veranstaltung in dessen Rahmen das Projekt lief]
festival_teaser: internationales Festival für computergestützte Kunst [Beschreinung der Veranstaltung]
festival_link: http://cynetart.de/ [Link zur Veranstaltung]

participants: [Teilnehmer]
- Martin Herrmann 
- Deborah Schmidt
- Hannes Leitner
- weitere

---

[Beschreibungstext]
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet
```

