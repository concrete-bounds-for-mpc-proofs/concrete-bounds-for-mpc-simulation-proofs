Structure: 
 - case-studies contains
    - the auth-to-secure case study in auth-to-secure.ipdl
    - the DHKE-OTP case study in dhke-otp.ipdl
    - the multi-party coin toss case study in coin-toss.ipdl
    - the multi-party GMW case study in GMW-N.ipdl
 - the archive code.zip contains the source code 
 and the same case studies as in the folder case-studies. 
 To run them, extract the archive, cd to IPDL/src and run
  maude -no-banner -allow-files run-SpeX
 then at the resulting prompt enter  
  load dhke-otp.ipdl
 or 
  load auth-to-secure.ipdl  
 or
  load coin-toss.ipdl
 Note that the latter is a strict equality proof and therefore no bounds are displayed.
To run the multi-party GWM case study, cd to IPDL/src and run
 maude -no-banner -allow-files BaseGMWN.maude run-SpeX
then 
  load GMW-N.ipdl
The proof takes around 12 minutes so you will need to wait for a result.
