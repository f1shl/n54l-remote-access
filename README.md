# n54l-kvm-remote

## Prerequisites
- Git Repository klonen
- JRE Verison 1.6 für 32Bit herunterladen und installieren. Für den Test wurde die Version 1.6.0_45 verwendet
- Das Verzeichnis C:\Program Files (x86)\Java\jre6 in das Git Repository kopieren und in "jre" umbennen.
- Folgende Dateien von der RemoteAccessCard herunterladen:
  - http://IpAdress:80/software/avctKVMIOWin32.jar
  - http://IpAdress:80/software/avctKVM.jar
- Die avctKVM.jar Datei in das Git Repository kopieren.
- Die avctKVMIOWin32.jar Datei in das Git Repository kopieren und in avctKVMIOWin32.zip umbennen.
- Einen Ordner "lib" im Git Repository erstellen und das gerade erstellte Zip Verzeichnis dorthin entpacken

Die Ordnerstruktur sieht nun folgendermaßen aus:
|

|-jre

|-lib

 |-avctKVMIO.dll

|- avctKVM.jar

|- avctKVMIOWin32.jar

|- chromedriver.exe

|- StartKVM.py

- Open Powershell window in folder and install necessary python packages with: pip isntall -r requirements.txt

## Verbindung herstellen
- Powershell im Ordner öffnen und "python StartKVM.py" eintippen
