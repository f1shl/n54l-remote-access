# n54l-kvm-remote
This small python script can be used to establish the connection to the N54L Remote Access Card, without the need of downloading the java file manually of the remote access card webserver.
This script works as well for Windows 10.

Google Chrome must be installed as browser on the PC.
## Prerequisites
- Clone the respository
- Download the Java verison 1.6.045 (https://www.oracle.com/de/java/technologies/javase-java-archive-javase6-downloads.html) and install it
- Copy the directory *C:\Program Files (x86)\Java\jre6* into the git repository and rename it to *jre*
- Download the following files from the RAC webserver and copy them into the repository:
  - http://ipaddress:80/software/avctKVMIOWin32.jar
  - http://ipaddress:80/software/avctKVM.jar
- Rename the file *avctKVMIOWin32.jar* to *avctKVMIOWin32.zip*
- Create a folder called *lib* and unzip the Zip file to it. 
The folder structure should now look the following:  
|-jre  
|-lib  
&nbsp;&nbsp;|-avctKVMIO.dll  
|- avctKVM.jar  
|- avctKVMIOWin32.jar  
|- StartKVM.py  

- Open Powershell window in folder and install necessary python packages with: *pip install -r requirements.txt*

## Create a connection
- Open a powershell window within the repository root folder
- Type *python StartKVM.py* into it
- IP address, user name and password will be asked
- The remote connection should now be established
