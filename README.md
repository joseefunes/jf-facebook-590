# jf-facebook-590
1. (Required) Vulnerability Name or ID
  - [ ] Summary: After find out the Xss was able to be executed in WP version 4.2 I used WPScan to research for any available link to help me solve this issue. After the scan, I found out a script that after inputting a total of 64K data in the comment box; approximate 66,000 character, will overload the max input in the comment box, letting me execute a Xss script.
    - Vulnerability types: Xss
    - Tested in version:4.2
    - Fixed in version: 4.2.1 
  - [ ] GIF Walkthrough: https://media.giphy.com/media/2tKDARPsofd85XXUnh/giphy.gif
  - [ ] Steps to recreate: first I used the script provided from the web site listed below, I modify the msg to show when script gets execute , then I remove a part of the code ( ..[64K]..) and add characters until reached 64k worth of input. After got enough characters  click submit comment and boom!! Xss is applied
  - [ ] Affected source code:
    - [Link 1]( https://klikki.fi/adv/wordpress3.html )

2. (Required) Vulnerability Name or ID
  - [ ] Summary: after scanning using WPScan I found out that theirs an easy way to find out which version of WP is in use. By adding readme.html after .com/ I was able to find out the version used.
    - Vulnerability types: fingerprint
    - Tested in version:4.2
    - Fixed in version: --
  - [ ] GIF Walkthrough: https://media.giphy.com/media/874IogoEGFngiJdSDd/giphy.gif
  - [ ] Steps to recreate: first I used WPScan to find any possible vulnerability, then I found out that there is an access to find the version of the web site ( WP) just by adding (readme.html) after  (http://wpdistillery.vm/) 


3. (Required) Vulnerability Name or ID
  - [ ] Summary: I used WPSCan to find a possible vulnerability using SQL injection. I found one that after inputting it in the comment box what makes is that will approve every comment post it after that injection approval.
    - Vulnerability types: SQLI
    - Tested in version:4.2
    - Fixed in version: 4.2.4
  - [ ] GIF Walkthrough: https://media.giphy.com/media/42ByiTnW0jTZVAgexm/giphy.gif 
  - [ ] Steps to recreate: first is to find the proper SQL injection after that wait until is approved by the administrator. Once approved any comment from that user will be posted without an approval.
  
    - [Link (https://github.com/WordPress/WordPress/commit/70128fe7605cb963a46815cf91b0a5934f70eff5 )

    

