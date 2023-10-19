# Information PC Hardware Teil 1
### Komponenten eines Arbeitsplatzcomputers unterscheiden
Mitarbeiter in IT-Berufen können nicht alle Informationen zu allen Komponenten ständig auf abruf bereit halten. Das ist schlichtweg nicht möglich, aber es ist wichtig zu Wissen wo man diese Information schnell findet.

### Zentraleinheit, Mainboard und Betriebssysteme
Die Zentraleinheit eines Computer ist das Mainboard des Computers. Auf das Mainboard werden verschiedene Komponenten installiert z.B die Prozessor(CPU), mit das wichtigste Teil auf einem Mainboard. Hinzu kommen noch weitere Teile wie RAM (Random Access Memory),  GPU (Graphical Processing Unit), SSD/HDD (Solid State Drive) (Hard Disk Drives), Power Supply (PS). 
- Anwendung sendet Daten
- CPU bearbeitet die Daten 
- RAM ist das Kurzzeitgedächtnis des Computers, Daten gehen nach ausschalten verloren.
- CPU hat direkten Zugriff auf RAM um Informationen abzurufen

Damit der PC startet hat er einen Read Only Memory (ROM) auf dem Mainboard der das BIOS(Basic Input Output System) oder UEFI (Unified Extensible Firmware Interface) und ruft anschließend auf einer Festplatte das gespeicherte Betriebssystem auf. Damit die Programme konfliktfrei bearbeitet werden können gibt es einen Taktgeber der von der CPU gesteuert wird (Prozessoruhr, Clock, CLK).

Es gibt verschiedene Betriebssysteme (OS; Operating System) für Arbeitsplätze, die bekanntesten wären Microsoft Windows, Linux, Unix (Apple) oder Android(Linux abkömmling). Sie unterscheiden sich in Bedienoberfläche, Sicherheitsmanagement und Apps. Um weitere Betriebssysteme zu nutzen können wir diese Virtualisieren. VMM (Virtual Machine Monitor) wurden dafür entwickelt. Dadurch können wir z.B von einem Windows Host ein weiteres Gastsystem wie Linux(Ubuntu,Debian) oder Unix System benutzen. Das Gastsystem wird oft als Virtuelle Maschine bezeichnet.

`Um ein Betriebssystem zu virtualisieren brauchen wir oft eine Virtualisierungssoftware aka Hypervisor (Aufseher). Es gibt verschiedene Hypervisor wie z.B HyperV, WSL(Windows-Subsystem), KVM(Kernelbased Virtual Machine), VMware.


### Kompetenzcheck
1. Erläutern Sie mit eigenen Worten, was man unter ZE, CPU, BIOS, CLK, Betriebssystem, VMM, Apps versteht.
	1. ZE ist die Zentraleinheit des Computers und wird auch Mainboard/Motherboard genannt
	2. CPU ist die Central Processing Unit aka Prozessor und ist für die Berechnungen zuständig
	3. BIOS ist das Basic Input Output System und ist ein Vorgänger vom heutigen UEFI. Es lädt Firmware welche für den Start des Computers notwendig sind um anschließend ein Betriebssystem zu laden.
	4. CLK gibt die Taktgeschwindigkeit der CPU an, mit welcher Programmbefehle bearbeitet werden.
	5. Betriebssystem bieten die Bedienoberfläche und Programme. Beispiel hierfür sind Windows, Linux, Unix
	6. VMM auch Virtual Machine Monitor genannt, bietet eine Soft/Hardware Lösung um ein Gastsystem wie z.B Linux auf einem Windows Rechner zu virtualisieren.
	7. Apps werden auch ganz einfach Computerprogramme bezeichnet. Sie bieten eine Funktion um es für den Anwender angenehmer zu machen Probleme zu lösen.

2. Was ist richtig, wer hat die schnellste Antwort ?
	1. CPU ist das Motherboard insgesamt
		1. Nein, die CPU ist der Prozessor, welcher Programmbefehle bearbeitet. Das Mainboard ist die Hauptplatine des Computer, welche zusätzliche Komponenten verbindet. 
	2. CLK bedeutet Cental Large Canceling
		1. Nein, CLK bedeutet Clock oder auch Clockrate. Sie gibt die Taktgeschwindigkeit des Prozessors vor.
	3. UEVI ist ein anderes Wort für BIOS
		1. Nein, UEVI gibt es so nicht. Es heißt wenn UEFI was Unified Extensible Firmware Interface beudetet.
	4. Mit einer VMM können mehrere Betriebssysteme mit entsprechenden Programmen gleichzeitig laufen.
		1. Ja wenn dafür die Hardwarekapazität vorhanden ist. Mehrere VM laufen zu lassen erfordert eine starke CPU und viel RAM.
	5. Systeminformationen erhält man über das Office Programm
			1. Nein, Systeminformationen erhält man über Windows(Sysinfo) oder über Linux mit dem Befehl Neofetch oder cat /proc/cpuinfo


### Hauptplatine, Mainboard und die Komponenten beschreiben
Das Mainboard ist die Hauptplatine, alle weiteren Komponenten werden auf diese aufgebracht. Das BIOS ist für den Startvorgang des Computers zuständig. Der Chipsatz ist das wichtigste Teil, denn er ist für die Kommunikation der  Hardware Komponenten zuständig. Die Herstellung eines Mainboards wird meistens von großen Chip und Prozessor Herstellern übernommen wie z.B Intel, AMD, Asus, ASRock, MSI. Der Formfaktor eines Mainboards gibt die Größe an. Die bekanntesten sind ATX und ITX. Bei einem Kauf von einem Mainboard muss auf die Kompatibilität der einzelnen Komponenten geachtet werden, wie z.B der CPU. Mainboards haben verschiedene Sockel wie z.B AM4, AM5, Intel 2011 - 2066, nur die jeweilige CPU Generation passt auf den Sockel. 


### Kompetenzcheck
1. Formfaktor des Mainboards
	1. Die gängisten sind ATX und ITX. Bei einem Formfaktor sprechen wir von der Größe und der Form des Mainboards
2. Chipsatz
	1. Der Chipsatz ist für die Kommunikation der Hardware Komponenten zuständig.
3. Sockel
	1. Der Sockel des Mainboards gibt an, welche CPU Generation kompatibel mit diesem ist. Ein Beispiel dafür wäre Intels 2066 oder AMDs AM4/5
4. Prozessor
	1. Der Prozessor ist für die Bearbeitung der Programmbefehle zuständig. Der Takt gibt an wie viele Programmbefehle bearbeitet werden können.
5. Steckplatz
	1. Bei einem Steckplatz reden wir von z.B PCIe x16 für GPUs oder RAM-Steckplätze für den Arbeitsspeicher. Diese finden wir auf dem Mainboard
6. GPU
	1. Auch Graphical Processing Unit genannt und ist für die Bildverarbeitung zuständig. Programme mit besonderer Anforderung nutzen diese wie Spiele, Videobearbeitungsprogramme, 3D Rendering Programme.
7. Cache
	1. Cache ist der Schnelle Speicher einer CPU. Er ist noch schneller als RAM.


### Kompetenzcheck
1. Erläutern Sie mit eigenen Worten, was man vereinfacht unter nm, Multi Core, Kühler, Parallelisierung, Taktfrequenz, MHz, Multi-Threading, Turbo boost, GPGPU versteht.
	1. nm ist die Maßeinheit von Chips. Umso kleiner umso Leistungsstärker und Energieeffizienter
	2. Multi Core ist eine CPU mit mehreren Kernen.
	3. Kühler bezeichnet man den Kühler, welcher auf der CPU sitzt. Es gibt Luft- und Wassergekühlte Kühler.
	4. Parallelisierung ist ein intelligenter und effizienter Weg, Wartezeit zu verkürzen und die CPU besser zu nutzen.
	5. Taktfrequenz heißt umso höher umso schneller arbeitet die CPU, was aber zu mehr Temperatur führt. Es wird auch mehr Strom benötigt.
	6. MHz ist die Einheit mit dem der Takt einer CPU bestimmt wird.
	7. Multi-Threading ist eine Art von Parallelisierung
	8. Turbo boost ist ein automatisches Overclocking. Intel und AMD CPUs nutzen diese Technologie
	9. GPGPU ist eine Programmierschnittstelle Berechnungen über die GPU laufen zu lassen.


### Kompetenzcheck
1. Erläutern Sie mit eigenen Worten, was man vereinfacht unter RAM, FSB, ECC, DIMM, SDRAM, MT, Latenz, QLZ, NAND versteht
	1. RAM bedeutet Random Access Memory und ist langsamer als der Cache Speicher auf der CPU. Die Festplatte führt ein Programm aus und wird in den RAM geladen. Die Geschwindigkeit wird in Megatransfer/Second berechnet.
	2. FSB auch Front Side Bus genannt. Er verbindet Prozessor, Chipset, DRAM und Grafikcontroller. 
	3. ECC bedeutet Error Correcting Code und hilft Speicherfehler zu minimieren.
	4. DIMM bedeutet Dual In Line Memory Module und wird häufig in Servern und Desktop-PCs gefunden. Es ist der Formfaktor vom RAM
	5. SDRAM bedeutet Synchronous Dynamic Random Access. Er speichert Daten synchron zum Speicher-Bus. Der Takt wird vom System-Bus vorgegeben.
	6. MT heißt Megatransfer und ist die Einheit in der RAM Programm aus dem Speicher lädt.
	7. Latenz ist die Zeit die der Speicher benötigt um auf einen Befehl zu reagieren.
	8. QLZ bedeutet Quad-Leve-Zellen und ist die neuste Technologie in der Flash-Speicherarchitektur. 
	9. NAND bezeichnet einen Typ von Flash-Speicher.

2. Was ist richtig?
	1. Die geschwindigkeit des RAM wird in MT/s gemessen.
		1. Richtig, die Geschwindigkeit des RAM wird in MT/s gemessen.
	2. SO-RAM sind für Desktopsysteme.
		1. SO-RAM wird eher in Notebooks und Laptops eingesetzt da sie vom Formfaktor kleiner sind
	3. Derzeit ist das DDR4 das RAM mit dem höchsten Energieverbrauch.
		1. Das stimmt nicht, da die neusten Technologien immer Energieeffizienterwerden, und höhere Taktraten zulassen.
	4. Mit DDR3 können 32GB erreicht werden.
		1. Wenn das Mainboard genügend Steckplätze hat ist es möglich sogar mehr als 32GB zu verbauen. Der maximale Speicher eines DDR3 Riegel ist 16GB.
	5. DDR3 gibt es nur in 2-GB, 4-GB und 8-GB Riegeln
		1. Nein, es gibt auch einen 16GB Riegel, höher geht es nicht.
	6. SSD sind magnetische Flashspeicher
		1. Das stimmt, eine SSD ist ein elektronischer Speicher.
	7. Latenz bedeutet Reaktionsgeschwindigkeit (des Speichers)
		1. Das stimmt, umso niedriger die Latenz, umso schneller kann der Speicher auf Befehle reagieren

### Kompetenzcheck
2. Was ist richtig?
	1. PCIe-Steckplätze sind für RAM-Karten und RAM-Riegel zu verwenden
		1. Nein, dafür gibt es seperate Steckplätze. PCIe-Steckplätze sind für GPUs oder Netzwerkkarten
	2. bei DIMMS ist beim Einbau auf die Einkerbung zu achten.
		1. Nein, das ist eher bei einem Sockel für die CPU der Fall.
	3. SATA-Anschlüsse sind für Festplatten vorgesehen.
		1. Das ist richtig, dort können wir verschiedene Arten von Festplatten anschließen.
	4. je mehr lanes, desto geringer ist die Datenrate/s
		1. Genau das Gegenteil ist der Fall.
	5.  Der M.2-Port löst den SATA-Port ab
		1. Im Consumer Sinne wird die M2 irgendwann die SATA-Festplatten ablösen. Aber etwas wie ein SATA-Port gibt es nicht.
	6. Die Datentransferrate wird in GB/s gemessen
		1. Die Datentransferrate kann in MB/s oder GB/s, sowie Mbit/s oder Gbit/s gemessen werden.
	7. USB-Anschlüsse gibt es bis zur Spezifikation 2.0
		1. Nein, es gibt bereits USB 3.x Gen 1-2