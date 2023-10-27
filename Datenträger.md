**Aufgabe 1:**
Was ist die kleinste Einheit einer Festplatte, die das Betriebssystem direkt ansprechen kann?
- Die kleinste Einheit ist das Cluster (512Byte)

**Aufgabe2:**
Warum werden Sektoren zu Clustern zusammengefasst? Nennen Sie Vor- und Nachteile großer Clustergrößen.
- Da das Betriebssystem nicht auf einzelne Bits und Bytes zugreifen kann, werden Zusammenfassungen von Datenblöcken(Cluster) verwendet. Cluster können zwischen 512Byte und 32.768Byte groß sein. Der Vorteil ist, das schnell auf Dateien zugegriffen werden kann und die Datei schneller lädt.


**Aufgabe3:**
Welche Daten (Cluster, Sektor, Zylinder, Partition) können mit einer Umdrehung der Festplatte
eingelesen werden?
- Eine Spur

**Aufgabe 4:**
Warum werden Festplatten partitioniert?
- Festplatten werden partitioniert, um z.B Bootloader, Spiele, Programme, Dateien zu trennen.

**Aufgabe 5:**
Beim Partitionieren von Festplatten kommt entweder MBR oder GPT zum Einsatz.
**a)** Wie viele Partitionen können beim MBR-Verfahren angelegt werden?
- Vier Partitionen

**b)** Wie sind die maximalen Partitionsgrößen bei MBR bzw. GPT?
- 2TB ist die maximale Partitionsgröße

**Aufgabe 6:**
Welche Aufgabe hat das Dateisystem?
- Es ist für die Belegung der Cluster zuständig und verbindet die Cluster mit logischen Dateien. Es ist die Grundlage für Speichern, Löschen, Umbenennen von Dateien. Ohne das Dateisystem könnten wir außerdem die Metadaten (Größe, Datum) nicht auslesen und die Dateiattribute nicht einsehen/ändern. Desweiteren bietet es Sicherheitsfunktionen wie das Journaling/Logs.

**Aufgabe 7:**
Viele Geräte wie Digitalkameras, Smartphones, FritzBoxen oder Smart-TVs unterstützen als Datei-
system FAT32.
**a)** Warum ist FAT32 so weit verbreitet?
- Es wurde von Microsoft entwickelt und arbeitet mit 32Bit. Die maximale Dateigröße beträgt 4GB, mit einer maximalen Clustergröße von 32KB. Für die meisten Verbraucher/Nutzer ist dies ausreichend.
**b)** Welche zwei Punkte muss man beachten, wenn man Dateien von einem NTFS- Dateisystem (Festplatte) auf ein FAT32-Dateisystem (z. B. USB-Stick) kopiert?
- Das die maximale Dateigröße nicht überschritten wird, und die maximale Länger des Dateinamens nicht 255Zeichen überschreitet(Was eher selten der Fall ist). 

**Aufgabe 8:**
Ein Dienstprogramm zeigt folgende Informationen zu einer Festplatte an:
**Größe:** 76,7 GiB
**Zylinder:** 39420
**Sektoren pro Spur:** 255
**Bytes pro Sektor:** 512

- 8 Magnetscheiben


**Aufgabe 1:**
Nennen Sie mindestens fünf Kenngrößen, die bei der Auswahl einer geeigneten Festplatte eine
Rolle spielen, und erläutern Sie diese kurz.
- RPM(Rounds Per Minute), Speicherplatz, Sektorgröße, Sektoren pro Spur, Zylinder

**Aufgabe 2:**
Nennen Sie die drei gängigsten Baugrößen von Festplatten und deren typischen Verwendungs-
zweck. Was genau wird mit der Größe angegeben?
- 3,5" SATA HDD -> Desktop Computer, sowie im Serverbereich
- 2,5" SATA HDD -> Ursprünglich für Notebooks entwickelt, findet aber auch Verwendung in Desktop Computer und Servern
- M.2 SSD -> Finden Platz in Desktop Computer und Notebook. Hat größtenteils die HDD abgelöst.

**Aufgabe 3:**
Welche Drehzahlen sind heute bei Magnetfestplatten üblich? Warum ist die Festplatte mit der
höchsten Drehzahl nicht immer optimal?
- 7200 bis 15.000 Rounds per Minute sind die gängigsten Magnetfestplatten. Umso höher die RPM, desto lauter arbeitet die Festplatte. 

**Aufgabe 4:**
Erläutern Sie kurz und mit eigenen Worten folgende Fachbegriffe im Zusammenhang mit
Magnetfestplatten: Köpfe (Heads), Sektor, Spur, Cluster, Zylinder, Headcrash, CHS, LBA.
- **Köpfe:** Ist für das Auslesen zuständig. 
- **Sektor:** 
- **Spur:**
- **Cluster:** Besteht aus mehreren Blöcken und bietet eine schnellere Ladezeit und Lesegeschwindigkeit
- **Zylinder:** Besteht aus mehreren Scheiben und bestimmt somit die Größe der Festplatte
- **Headcrash:** Ist eine Beschädigung der Oberfläche auf einer Magnetscheibe
- **CHS:** Eine veraltete Methode zum Ansprechen einer Festplatte. Ist für die Adressierung der Festplatte zuständig, wurde durch LBA abgelöst.
- **LBA:** Adressierungsmethode der Festplatte. Im Gegensatz zu CHS wird unabhängig der Festplattengeometrie adressiert.

**Aufgabe 5:**
Nennen Sie mindestens vier Bestandteile einer SSD.
- Cache -> ist ein flüchtiger Speicher
- Flash Array -> Storage-Lösung ohne verschleiß
- Garbage Collection -> Prüft ob auf dem Betriebssystem gelöschte Dateien noch auf der SSD liegen und verwirft diese anschließend.
- Anschluss -> M.2, SATA, PCIe

**Aufgabe 6:**
Welche Anschlüsse sind z. T. bei SSDs üblich, und wo werden sie üblicherweise verwendet?
- SATA 6G
- M.2
- PCIe
- SATAe

**Aufgabe 7:**
Welche Gemeinsamkeiten und welche Unterschiede gibt es bei Magnetfestplatten und SSDs?
- Speicherplatz
- Anschlüsse
- Bauform

**Aufgabe 8:**
Welche Argumente sprechen bei Notebooks für den Einsatz von SSDs?
- Ladezeit
- Lautstärke
- Bauform

**Aufgabe 9:**
Erläutern Sie kurz und mit eigenen Worten folgende Fachbegriffe im Zusammenhang mit SSDs:
Controller, SLC, MLC, TLC, Löschzyklus, Wear Leveling, Over Provisioning.
- **Controller:** Steuert den Datenfluss
- **SLC:** Single Level Cell, speicher ein Bit pro Zelle und ist somit  und arbeiten schnell.
- **MLC:** Multi Level Cell, speichert zwei Bit pro Zelle, sind langsamer und halten weniger lange.
- **TLC:** Triple Level Cell, speichert drei Bit pro Zelle, verkraften aber nur 3.000 Schreibzyklen und sind somit kurzlebig.
- **Löschzyklus:** Je nach Fertigungsart halten die Speicherzellen von SSDs nur eine begrenzte Anzahl an Schreib und Löschzyklen aus. 
- **Wear Leveling:** Gleichmäßige Verteilung von Daten auf den Speicherzellen.
- **Over Provisioning:** Reservierung von Speicherplatz und kommt bei defekten Speicherzellen zum Einsatz

**Aufgabe 10:**
Bei der Einrichtung einer neuen Festplatte ist ein mehrstufiger Einrichtungsprozess nötig.
Beschreiben Sie dazu folgende Fachbegriffe: Partition, MBR, GPT
- **Partition:** Verschiedene Regionen/Bereiche einer Festplatte
- **MBR:** Master Boot Record für ältere BIOS Systeme
- **GPT:** GUID Partition Table ist UEFI basiert. Für neue BIOS Systeme
