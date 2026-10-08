---
title: "Ressourcen und Metadatenprofile"
teaching: 10 # teaching time in minutes
exercises: 10 # exercise time in minutes
---

:::::::::::::::::::::::::::::::::::::: questions 

- Wie werden Ressourcen erstellt?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Legen Sie eine Resource an
- Wählen und befüllen Sie ein Metadatenschema

::::::::::::::::::::::::::::::::::::::::::::::::


## Schritt 1: Ressourcentyp festlegen 

Mit dem Ressourcentyp legen Sie fest, wo Ihre Daten gespeichert sein sollen. So gibt es z.B. die Möglichkeit, Daten über Coscine auf dem DataStorage.nrw zu speichern oder nur einen Datensatz zu verlinken, der bereits an einem anderen Ort gespeichert ist (z.B. GitLab).

-------       ---------------------------------------------------
Web           Web-Ressource des Datastorage.nrw. Bis zu 100 GB Speicherplatz ist kein Antrag erforderlich. Auf Antrag auch mehr Speicherplatz möglich. Zugriff nur über Webinterface oder API. Dies ist der "Standard" Ressourcentyp wenn Ihre Daten in Coscine gespeichert werden. 
S3            S3-Ressource des Datastorage.nrw. Für die S3-Ressource muss ein Antrag gestellt werden. Es sind bis zu 125 TB Speicherplatz pro Speicherplatz-Antrag möglich. Zugriff erfolgt über Webinterface, API oder S3-Client.
WORM          WORM-Ressource des Datastorage.nrw für besonders vor Manipulation zu schützende Daten. Daten können nach dem Speichern nicht mehr gelöscht oder verändert werden (Write Once Read Many). Für die WORM-Ressource muss ein Antrag gestellt werden. Es sind bis zu 125 TB Speicherplatz möglich. Dieser Typ ist nur in Sonderfällen relevant. Beraten Sie sich mit ihrem lokalen Coscine Support wenn Sie überlegen eine WORM Ressource zu beantragen. 
GitLab        Sie können ein GitLab-Projekt mit Coscine verknüpfen und so alle Dateien, die im GitLab Projekt liegen, in Coscine mit Metadaten beschreiben. Die Daten verbleiben weiterhin in GitLab, die Metadaten werden in Coscine gespeichert. Da bei dieser Resource die Daten selbst nicht in Coscine gespeichert werden kann sie auch genutzt werden wenn Sie nicht Teil einer Institution sind, die Speicher in Coscine zur Verfügung stellt.
Linked Data   Sie können Dateien, die an einem anderen Speicherort liegen, mit einem persistenten Link in Coscine verknüpfen und dort die Dateien mit Metadaten beschreiben. Auch hier bleiben die Daten am ursprünglichen Speicherort. Da bei dieser Resource die Daten selbst nicht in Coscine gespeichert werden kann sie auch genutzt werden wenn Sie nicht Teil einer Institution sind, die Speicher in Coscine zur Verfügung stellt.
-------       ---------------------------------------------------

## Schritt 2: Metadatenprofil festlegen

Im zweiten Schritt wählen Sie ein Metadatenprofil. Dies bestimmt die Eingabefelder für die Metadaten (z.B. Ersteller:in, Erhebungsmethode, Datentyp, Lizenz…). Einige Profile und Standards sind in Coscine bereits vorgegeben (z.B. BASE oder EngMeta). Wenn Sie kein passendes Profil für Ihre Daten finden, dann können Sie auch ein eigenes erstellen und beantragen.

::: callout

Das ausgewählte Metadatenprofil kann im Nachgang nicht mehr geändert werden. Wenn Sie das Profil später wechseln wollen müssen Sie die Resource löschen und von vorne beginnen. Es lohnt sich also, sorgfältig zu planen!

:::

## Schritt 3: Ressourcenmetadaten ausfüllen 

Im letzten Schritt müssen Sie nun noch ein paar Informationen über die Ressource eingeben: 

---------------------------------      ---------------------------------------------------
Ressourcenname                         Eindeutiger Name der Ressource
Anzeigename                            Kurzer Anzeigename der Ressource
Ressourcenbeschreibung                 Beschreibung von Inhalt und Zweck der Ressource
Disziplin                              Entspricht der [DFG-Fachsystematik](https://www.dfg.de/resource/blob/172316/5863ef132d178054609f74940f6a27c9/fachsystematik-2016-2019-de-grafik-data.pdf) (Mehrfachauswahl möglich)
Projektschlagwörter                    Zur besseren Einordnung und Suchbarkeit der Ressource
Sichtbarkeit                           Bei der Einstellung „public“ können alle Nutzenden von Coscine die (Meta-)Daten finden. Sie haben keinen Zugriff auf die Daten selbst, können Sie jedoch bei Interesse kontaktieren.
Lizenz                                 Für alle Dateien der Ressource kann eine Lizenz ausgewählt werden. Für Forschungsdaten werden die Creative Commons Lizenzen (CC-Lizenzen) empfohlen. Weitere Infos finden Sie auf [forschungsdaten.info](https://forschungsdaten.info/themen/rechte-und-pflichten/forschungsdaten-veroeffentlichen/creative-commons-lizenzen/).
Interne Regeln zur Nachnutzung         Besondere Regeln und Informationen zur Nachnutzung der Dateien innerhalb der Organisation (z.B. Wie soll mit den Daten umgegangen werden, wenn der/die Projektleiter:in nicht mehr da ist?)
---------------------------------      ---------------------------------------------------


::::::::::::::::::::::::::::::::::::::: challenge

**Falls Speicherplatzressourcen an Ihrer Institution verfügbar sind:** 

- Erstellen Sie in Ihrem Projekt eine Ressource vom Typ „Web“.


**Falls Speicherplatzressourcen an Ihrer Institution <u>nicht</u> verfügbar sind:**

- Erstellen Sie in Ihrem Projekt eine Ressource vom Typ „Linked Data“. 


::: hint

Verwenden Sie das Metadatenprofil „Base Profile“.

:::

::: hint

Verwenden Sie bei Bedarf diese Metadaten:
Ressourcenname: Basisdaten

Ressourcenbeschreibung: Der Datensatz enthält alle Haltestellen im AVV-Verbundgebiet auf Ebene der Masten, soweit verfügbar mit GlobalID. Es sind nur Haltestellen in der Städteregion Aachen, dem Kreis Düren und dem Kreis Heinsberg enthalten. Die Koordinaten sind im Format Gauß-Krüger 2 (EPSG:31466) gepflegt.

Sichtbarkeit der Metadaten: Project Members

Lizenz: CC BY 4.0 (Attribution)

Interne Regeln zur Nachnutzung: Keine

:::

::::::::::::::::::::::::::::::::::::::::::::::::::
