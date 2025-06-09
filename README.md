Structure: 
 - case-studies contains
    - the auth-to-secure case study in auth-to-secure.txt
    - the DHKE-OTP case study in dhke-otp.txt
    - the multi-party coin toss case study in coin-toss.txt
    - the multi-party GMW case study in GMW-N.txt
 - the archive code.zip contains the source code 
 and the same case studies as in the folder case-studies. 
 To run them, extract the archive, cd to code/src and run
  `maude -no-banner -allow-files run-SpeX`
 then at the resulting prompt enter  
 `load dhke-otp.txt`
 or 
  `load auth-to-secure.txt` 
 or
  `load coin-toss.txt`

 Note that the latter is a strict equality proof and therefore no bounds are displayed.
 
To run the multi-party GWM case study, cd to code/src and run
 `maude -no-banner -allow-files BaseGMWN.maude run-SpeX`
then 
  `load GMW-N.txt`
The proof takes around 12 minutes so you will need to wait for a result.

In the main folder of the repository, run

`unzip -d maude Maude-linux.zip`

`unzip code.zip`

`export MAUDE_LIB=./maude/:./code/src`

We have tested these steps on Ubuntu Linux 24.04.
