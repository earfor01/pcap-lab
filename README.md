set1.pcap

1. How many packets are there in this set?

465

2. What protocol was used to transfer files from PC to server?

FTP

3. Briefly describe why the protocol used to transfer the files is insecure?

when securing the connection, ftp sends data in plaintext, which means anyone snooping your connection can grab username and password information

4. What is the secure alternative to the protocol used to transfer files?

SFTP

5. What is the IP address of the server?

192.168.1.4

6. What was the username and password used to access the server?

username: broken

password: r3wt

7. How many files were transferred from PC to server?

4

8. What are the names of the files transferred from PC to server?

48b.jpg

522.jpg

639.jpg

b29.jpg

9. Extract all the files that were transferred from PC to server.



These files must be part of your submission!



set2.pcap

Scenario: Someone has been covertly sending pictures to another person electronically. You intercepted communications at a good time and noticed data seemed to be transmitted in-the-clear. However, the data looks weird for a single picture, unlike anything you have seen before. Reconstruct the picture that was sent covertly. HINT: take a look at the last packet and notice the payload data.

10. How many packets are there in this set?

4

11. To what service or protocol did the sender use to covertly send images? Briefly describe your answer.

tcp w/ base64 encoding

12. Briefly describe how you were able to reconstruct the image from the packets.

Copy tcp payloads in files and decode from base64

13. Who is in the picture?

Ben Hescott





set3.pcap

14. How many packets are there in this set?

80525

15. How many plaintext username-password pairs are there in this packet set? Please count any anonymous or generic accounts.

2

user: nagiosadmin pass:Vid30Plus! info:12.227.41.123/nagios/ 
TCP 80 12.227.41.123
hypertext trader protocol
port 80
server Apacher/2.2.15
Nagios access
user: nab01620@nifty.com pass:Nifty->takirinl
	tcp port 143 210.131.4.155
  
16. Briefly describe how you found the username-password pairs.

I converted the cap into an etterlog file and ran etterlog -p on it

17. For each of the plaintext username-password pair that you found, identify the protocol used, server IP, the corresponding domain name if possible (e.g., google.com), and port number.



IMPORTANT NOTE: PLEASE DO NOT LOG ON TO THE WEBSITE OR SERVICE ASSOCIATED WITH THE USERNAME-PASSWORD THAT YOU FOUND!



18. Of all the plaintext username-password pairs that you found, how many of them are legitimate? That is, the username-password was valid, access successfully granted? Please do not count any anonymous or generic accounts.

1 of the two I found was a valid user/password  pair, and access was successfully wanted in that transaction 



set4.pcap

19. How many plaintext username-password pairs are there in this packet set? Please count any anonymous or generic accounts.

1

20. For each of the plaintext username-password pair that you found, identify the protocol used, server IP, the corresponding domain name if possible (e.g., google.com), and port number.

177.39.17.52 port 143 tcp

user:wanders@e-netsecueity.com.br pass:1052wmc12$$



IMPORTANT NOTE: PLEASE DO NOT LOG ON TO THE WEBSITE OR SERVICE ASSOCIATED WITH THE USERNAME-PASSWORD THAT YOU FOUND!

21. Of all the plaintext username-password pairs that you found, how many of them are legitimate? That is, the username-password was valid, access successfully granted? Please do not count any anonymous or generic accounts.

1

22. Provide a listing of all IP addresses with corresponding hosts (hostname + domain name) that are in this PCAP set. Describe your methodology.

Converted the cap to an ettercap file, ran a search to show Ip addresses 





