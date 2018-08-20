Move and run the entire AutomationScripts folder into the same directory as CS client and teamserver

In order to configure the redir, MSF, CS Teamserver, CS Client, and run proxychains nmap commands use SetupScript.py

Run SetupScript.py with python3.6 (others may work but havn't been tested).


Beacon_Initial.cna	- When a beacon is initiated these commands are run at second checkin.
C2.profile		- Amazon C2 profile with a sleep of zero.
elevate.cna		- Raffie Mudge's elevate kit. Upload to CS
Enum.py			- Proxychains netdiscover and Proxychains nmap commands. Should be enough to enumerate Quantico (will be prompted to run after SetupScript.py).
persistence.cna		- Raffie Mudge's persistence kit. Upload to CS.
SA.cna			- SA Commands. this may be broken into user SA and system SA in the future but for now it is one. Upload to CS.
SetupScript.py		- Configures redir, MSF, CS Teamserver, CS Client, and can kickoff Enum.py
Helper.cna		- System and User persistence notes as well as pass the beacon notes. Upload to CS.
QuickStart.py		- nano this and fill out then run to do run SetupScript.py faster
QuickStartBackground.py	- This is called by QuickStart.py to run setup quickly.


ASeriouslyREADME.txt	Helper.cna	QuickStart.py		SetupScript.py
Beacon_Initial.cna	elevate.cna	persistence.cna		SA.cna
C2.profile		Enum.py		QuickStartBackground.py  

