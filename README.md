Structure: 
 - case-studies contains
    - the auth-to-secure case study in auth-to-secure.txt
    - the DHKE-OTP case study in dhke-otp.txt
    - the multi-party coin toss case study in coin-toss.txt
    - the multi-party GMW case study in gmwn.txt
 - the archive Maude-linux.zip contains the version of Maude
 that we use to run the code with       
 - the archive code.zip contains the source code 
 and the same case studies as in the folder case-studies.

Installation:
In the main folder of the repository, run

`unzip -d maude Maude-linux.zip`

`unzip code.zip`

`export MAUDE_LIB=./maude/:./code/src`

To run the examples, do

  `maude/maude -no-banner -allow-files run-SpeX`

 then at the resulting prompt enter  
 
 `load code/dhke-otp.txt`
 
 or 
 
  `load code/auth-to-secure.txt` 
 
 or
 
  `load code/coin-toss.txt`

 Note that the latter is a strict equality proof and therefore no bounds are displayed.
 
To run the multi-party GWM case study, do

 `maude/maude -no-banner -allow-files BaseGMWN.maude run-SpeX`
 
 then 
 
  `load code/gmwn.txt`

The proof takes several minutes so you will need to wait for a result.

We have tested these steps on Ubuntu Linux 24.04.
