# n54l-kvm-remote

## Prerequisites
- Beziehen Sie sich eine JRE Verison 1.6 für 32Bit. Für den Test wurde die Version 1.6.0_45 verwendet - SIEHE Info
- Installieren Sie diese Version.
- Erstellen Sie ein neues Verzeichnis: Bsp. KVM
- Kopieren Sie folgendes Verzeichnis C:\Program Files (x86)\Java\jre6 in das zuvor erstellte KVM Verzeichnis und benennen es in jre um.
- Beziehen Sie folgende Dateien von der HP RAC aus ihrem Server:
  - http://<IPAdresseDerRAC>:80/software/avctKVMIOWin32.jar
  - http://<IPAdresseDerRAC>:80/software/avctKVM.jar

- Kopieren Sie die avctKVM.jar Datei in das KVM Verzeichnis.
- Kopieren Sie die avctKVMIOWin32.jar Datei in das KVM Verzeichnis und benennen die in avctKVMIOWin32.zip um.
- Erstellen Sie ein weiteres Verzeichnis im KVM Ordner mit dem Namen: lib
- Öffnen Sie nun die ZIP Datei und kopieren die avctKVMIO.dll Datei in das lib Verzeichnis.

- Von https://chromedriver.chromium.org/downloads dann den aktuellen Chromedriver herunterladen, der auch zum isntallieren Goolge Chrome Browser passt.

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
