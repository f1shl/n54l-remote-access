# n54l-kvm-remote

## Prerequisites
- Git Repository klonen
- JRE Verison 1.6 für 32Bit herunterladen und installieren. Für den Test wurde die Version 1.6.0_45 verwendet
- Das Verzeichnis C:\Program Files (x86)\Java\jre6 in das Git Repository kopieren und in "jre" umbennen.
- Folgende Dateien von der RemoteAccessCard herunterladen:
  - http://<IPAdresseDerRAC>:80/software/avctKVMIOWin32.jar
  - http://<IPAdresseDerRAC>:80/software/avctKVM.jar
- Die avctKVM.jar Datei in das Git Repository kopieren.
- Die avctKVMIOWin32.jar Datei in das Git Repository kopieren und in avctKVMIOWin32.zip umbennen.
- Einen Ordner "lib" im Git Repository erstellen und das grade erstellte Zip Verzeichnis dorthin entpacken
- Von https://chromedriver.chromium.org/downloads dann den aktuellen Chromedriver herunterladen, der auch zum installieren Goolge Chrome Browser von der Version passt.

Die Ordnerstruktur sieht nun folgendermaßen aus:
|
|-jre
|-lib
 |-avctKVMIO.dll
|- avctKVM.jar
|- avctKVMIOWin32.jar
|- chromedriver.exe
|- StartKVM.py

- Das Python package "selenium" über pip installieren

## Verbindung herstellen
- Im StartKVM.py File das Passwort, Nutzernamen und IP Adresse von der RemoteAccessCard einfügen.
- Powershell im Ordner öffnen und "python StartKVM.py" eintippen
