---
title: "Dateiupload, -download und -löschung"
teaching: 2 # teaching time in minutes
exercises: 0 # exercise time in minutes
---

:::::::::::::::::::::::::::::::::::::: questions 

- Wie kann ich Dateien in Coscine verwalten?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Führen Siedie folgenden Dateioperationen durch:
  - Hochladen
  - Herunterladen
  - Löscehn
  - Filtern

::::::::::::::::::::::::::::::::::::::::::::::::

## Upload

Sofern Sie eine "Web" Ressource erstellt haben, können Sie nun Daten über Coscine hochladen. Sie können entweder einzelne Datein hochladen oder auch mehrere Dateien auf einmal. Ziehen Sie die Datein einfach in die Weboberfläche von Coscine oder laden Sie die Dateien über die Buttons "Datei auswählen" und "Hochladen" hoch. Sobald Sie Ihre Daten ausgewählt haben, müssen Sie diese rechts mit Metadaten beschreiben. Danach können Sie die Daten final hochladen.

Wenn Sie eine "Linked Data" Ressource erstellt haben, können Sie keine Daten direkt in Coscine hochladen. Stattdessen verlinken Sie Daten, die in einer anderen Speicherumgebung gespeichert sind. Anschließend beschreiben Sie diese mit Metadaten. Nur die Metadaten sind nun in Coscine hinterlegt. Neben diesen beiden Varianten besteht auch die Möglichkeit, Daten automatisiert über die API hochzuladen oder über den S3-Client, wenn Sie eine S3-Ressource gewählt haben. Weitere Informationen zur [API](https://docs.coscine.de/de/api/api/) und zu [S3-Clients](https://docs.coscine.de/de/resources/s3-clients/) finden Sie in der Coscine-Dokumentation.

## Download und Löschen

Beim Download gilt das Gleiche wie beim Upload: Da die Daten bei der "Linked Data" Ressource extern gespeichert sind, können die Daten nicht in Coscine heruntergeladen werden. Inhalte von "Web", "S3", und "WORM"-Ressourcen können Sie hingegen herunterladen, indem Sie die gewünschten Daten über die Checkbox markieren, anschließend "Alle Dateien" auswählen und anschließend rechts auf "Herunterladen" klicken. 

Um Daten einer "Web" Ressource zu löschen, klicken Sie nach der Auswahl auf den Pfeil neben "Herunterladen", anschließend auf "Alle Dateien" und dann auf "Löschen". Bei Inhalten einer "Linked Data" Ressource gehen sie identisch vor. Allerdings entfernen Sie nicht den Datensatz (da sich dieser an einem externen Speicherort befindet), sondern nur die Verlinkung und die zugehörigen Metadaten.

::: callout

Gelöschte Inhalte können nicht wieder hergestellt werden.

:::

## Filtern

Über das Filtersymbol können Sie festlegen, welche Metadatenfelder in der Auflistung angezeigt werden sollen. Über die Suchleiste oberhalb der Liste können Sie nach Schlagwörtern suchen. Dies ist nützlich, wenn Sie beispielsweise alle Daten sehen möchten, die z.B. mit einer bestimmten Methode erhoben wurden. Dies setzt natürlich voraus, dass die Metadaten konsistent dokumentiert wurden.


::::::::::::::::::::::::::::::::::::::: challenge

**Falls Speicherplatzressourcen an Ihrer Institution verfügbar sind:** 

- Laden Sie einen Datensatz in Ihrer "Web" Ressource hoch und füllen Sie die Metadaten aus.
- Machen Sie sich mit der Filterfunktion vertraut.

**Falls Speicherplatzressourcen an Ihrer Institution <u>nicht</u> verfügbar sind:**

- Verlinken Sie einen Datensatz (der z.B. in [Sciebo](https://hochschulcloud.nrw/) gespeichert ist) in Ihrer "Linked Data" Ressource und füllen Sie die Metadaten aus.
- Machen Sie sich mit der Filterfunktion vertraut.

::::::::::::::::::::::::::::::::::::::::::::::::::
