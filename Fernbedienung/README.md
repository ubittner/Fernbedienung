# Fernbedienung

Zur Verwendung dieses Moduls als Privatperson, Einrichter oder Integrator wenden Sie sich bitte zunächst an den Autor.

Für dieses Modul besteht kein Anspruch auf Fehlerfreiheit, Weiterentwicklung, sonstige Unterstützung oder Support.  
Bevor das Modul installiert wird, sollte unbedingt ein Backup von IP-Symcon durchgeführt werden.  
Der Entwickler haftet nicht für eventuell auftretende Datenverluste oder sonstige Schäden.  
Der Nutzer stimmt den o.a. Bedingungen, sowie den Lizenzbedingungen ausdrücklich zu.

### Inhaltsverzeichnis

1. [Modulbeschreibung](#1-modulbeschreibung)
2. [Voraussetzungen](#2-voraussetzungen)
3. [Schaubild](#3-schaubild)
4. [Auslöser](#4-auslöser)
5. [Aktion](#5-aktion)
6. [PHP-Befehlsreferenz](#6-php-befehlsreferenz)

### 1. Modulbeschreibung

Dieses Modul schaltet eine Ziel-Variable oder führt ein Skript aus, wenn eine bestimmte Variable ausgelöst hat.  

### 2. Voraussetzungen

- IP-Symcon ab Version 6.1

### 3. Schaubild

```
+--------------------+                 +-----------------------+                 +-------------------+
| Fernbedienung (HW) |                 | Fernbedienung (Modul) |                 | Alarmzone (Modul) |
|                    |     Auslöser    |                       |     Aktion      |                   |
| Taste 1 - Variable |<----------------+ Auslöser 1            +---------------->| Vollschutz        |
|                    |                 |                       |                 |                   |
| Taste 2 - Variable |<----------------+ Auslöser 2            +---------------->| Hüllschutz        |
|                    |                 |                       |                 |                   |
| Taste 3 - Variable |<----------------+ Auslöser 3            +---------------->| Teilschutz        |
+--------------------+                 +-----------+-----------+                 +-------------------+
                                                   |
                                                   |
                                                   |                        +------------------------+
                                                   |                        | Alarmprotokoll (Modul) |
                                                   |                        |                        |
                                                   +----------------------->| Ereignisprotokoll      |
                                                                            +------------------------+
```

### 4. Auslöser

Das Modul Fernbedienung reagiert auf verschiedene Auslöser.  
Zusätzlich kann der Auslöser als Ereignisprotokoll in einem Alarmprotokoll protokolliert werden.

### 5. Aktion

Jedem Auslöser kann eine Aktion zugeordnet werden.

### 6. PHP-Befehlsreferenz

Es steht keine PHP-Befehlsreferenz zur Verfügung.