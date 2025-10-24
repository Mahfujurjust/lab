Question 1:
For Question 1, made a directory named Question1 as below:


Get the following file: 
wget https://github.com/SCH-IT-MurdochUni/NetworkingLabs/raw/refs/heads/main/Reusable_Learning_Objects/.test/.misc/lab_red.pcap.enc

Check the file: (file lab_red.pcap.enc will be generated) 







You can decrypt it by adapting the following command for your purposes:
sudo openssl enc -d -aes-256-cbc -in lab_red.pcap.enc -out lab_red.pcap.enc.tar.bz2 -k ‘2aT9134fnBwC$’
The encrypted file gets decrypted as below:


What percentage of the frames are 802.11 beacons? Answer to 1 decimal place but do not include a % sign
Open the wireshark as: sudo wireshark lab_red.pcap.enc.tar.bz2 

Filter it with ‘wlan.fc.type_subtype == 8’

Answer: You can see the result value at the bottom: 31.0 % and so is the answer.


What is the SSID used?
Answer: WirelessWPAtest


How many frames have been reported as a retransmission? Enter a number:
Answer: 50







Question 2:
Made Question2 directory:
And get the encrypted file as below:
wget https://github.com/SCH-IT-MurdochUni/NetworkingLabs/raw/refs/heads/main/Reusable_Learning_Objects/.test/.misc/pp.tar.bz2.enc
and file pp.tar.bz2.enc will be downloaded as below:

Decrypt the file:
Sudo openssl enc -d -aes-256-cbc -in pp.tar.bz2.enc -out pp.tar.bz2.enc.tar.bz2 -k ‘1&&jbjo7B2za’ 

Post decryption, you will need to untar the file as below: ‘tar -xvf pp.tar.bz2.enc.tar.bz2’ and two more files will be generated: 


Now open wireshark:
Go to Edit 🡪 Preference 🡪 Protocols 🡪 TLS 🡪 and select the sslkeylog.log file as below:

Click ok 
Recover all of the HTTP objects. The second-largest file has three words in it. Write these three words below all lower case with no spaces
Go to File 🡪 Export Objects 🡪 HTTP  ( Then sort by size ) and select the 2nd largest file and save it.

In ubuntu, open the saved image from deskop and you will see the image with three words that is drive your dream.


What frame number is this image requested in? Usually, in wireshark, the frame number is the left-most column. Requests from webpages are often HTTP Gets
Need to work on this: 13588


Question 3:
Get the file:





Decrypt the file:
Sudo openssl enc -d -aes-256-cbc -in eggtopia_anon_practice.pcap.bz2.enc -out eggtopia_anon_practice.pcap.bz2.enc.tar.bz2 -k ‘Psz#6j^3BqQl’

Open the file in Wireshark. If the data is encrypted, can you find the decryption key? You should use the password list here:
wget https://raw.githubusercontent.com/SCH-IT-MurdochUni/NetworkingLabs/refs/heads/main/Reusable_Learning_Objects/.test/.misc/leaked_password_list_clean.txt
A file named leaked_password_list_clean.txt will be generated as below:

If you open the leaked_password_list_clean.txt, you can see the list of words, and now from these word you need to decrypt a password:
Cat leaked_password_list_clean.txt



To get the decryption key, you will need to install aircrack-ng
I have aircrack-ng already installed:

To decrypt use the below command:
You will need to untar the secretarchive.tar.bz2 file and will get the file ‘data’ as below:






Question 4:








Sudo wireshark 2987.pcap.enc.tar.bz2
In wireshark filter it with UDP 🡪 right click in UDP under Protocol field 🡪 Follow 🡪 UDP Stream




Enter the contents of the flag. Enter as a string of ascii chars only, no spaces or newlines.
Answer: 10gQAZ%qgXX5


What is the source port in use to send this message:

Ans: port is 51822

There is a consistent time delay between messages, from the perspective of the packet capture, what is the delay between each of these messages: 

Answer: 20
We can see hat the time difference between the each record is 20 and hence answer is 20

