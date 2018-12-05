# How to access remote pvserver from your local machine}
  * There are two modes in which you can launch the ParaView server,pvserver and pvdataserver and pvrenderserver. 
  * In pvserver when all data processing and rendering are handled in the same parallel job. 
  * In second mode data processing is handled in one parallel job and the rendering is handled in another parallel job, pvdataserver and pvrenderserver programs, respectively.

## Prerequisite
 * Paraview 5.5 installed in remote and local machine
 * Putty or VNC viewer must be installed if windows is the local machine
 * MicrosftDesktop or VNC viewer must be installed if local machine is MAC
 * Download WinSCP
 
## Getting Started}
### Establish connection to remote machine
#### From Mac to Windows
##### Using VNC viewer/Microsft Desktop 
  *  Open Remote windows machine ->  Windows -> Computer/This PC -> Properties -> Remote settings -> Remote -> Check Allow Remote Assistance connection to this computer -> Choose Allow remote connections to this computer -> Apply -> OK
  *  Open command prompt -> ipconfig
  *  You can see the IPv4 Address -> copy it 
  *  Open your local Mac machine
  *  Download Microsoft Remote Desktop/VNC Viewer from app store
  *  open MS Remote Desktop
  *  Connection Name : Ricky Windows (can be anything)
  *  PC name : 192.168.88.17 (IP address of the windows machine you copied) 
  *  User name : \ipAddress{192.168.88.17/ricky}
  *  connect
  *  you are connected to Remote windows machine

##### Using Terminal

#### From Windows to Mac
  * Open your Remote -> System preferences -> Sharing -> check Remote Management -> You will see remote Management is on 
  * Copy the address mentioned <richie.cs.niu.edu>
  * Now open you windows local machine
  * You can download either putty or VNC viewer(Ill show both)

##### Using VNC viewer 
  * Open VNC viewer -> put <richie.cs.niu.edu> in the Server address bar -> connect 
  * click continue 
  * Enter the password you created in the remote machine
  * you are connected To Remote Mac
  * VNC is like a the Windows Remote Desktop feature where you can actually see the desktop environment on which you are working. You can control screen too.

##### Using putty
  * Open Winscp -> new site 
  * host name : richie.cs.niu.edu
  * username : ricky password : ********
  * login -> Upper left -> Open session in putty -> password 
  * you are connected to remote machine
  * Putty is an SSH client that you can use to connect to a machine running that service -- it's relatively secure but you only have a CLI and no GUI. 

### Establish connection to Paraview
  ** This is only required if you are accesing the remote machine via putty or terminal 
  * Go to mac default directory
  * ls -> cd Applications -> cd ParaView-5.6.0-RC1.app -> cd Contents -> cd bin 
  **cd Applications/ParaView-5.6.0-RC1.app/Contents/bin**
  * you should see the foloowing screen
  * figure
  
  

