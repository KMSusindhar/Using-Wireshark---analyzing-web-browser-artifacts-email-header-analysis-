# Using-Wireshark---analyzing-web-browser-artifacts-email-header-analysis
# NAME:SUSINDHAR K M
# REGISTER NO:212223040218

# AIM:
To use Wireshark to analyze web browser activities and inspect email headers from captured network traffic.

# DESIGN STEPS:
Step 1:
Launch Wireshark and start capturing traffic on the appropriate network interface.

Step 2:
Use filters like http, dns, or tcp.port == 80 to monitor web browser artifacts such as visited URLs, cookies, and user-agent strings.

Step 3:
Apply filters like smtp, pop, or imap to locate and analyze email header details (e.g., sender, receiver, subject) from email communications.

# PROGRAM:
Wireshark Web and Email Traffic Filtering Steps

# A. Capturing Traffic in Wireshark
Open Wireshark and start capturing on the active interface (Wi- Fi/Ethernet).
![image](https://github.com/user-attachments/assets/6b1b636e-30e6-4668-830f-ec9f35f29b4d)

# Analyzing Web Browser Artifacts
Analyze Queries:
# FILTER HTTP:

![image](https://github.com/user-attachments/assets/c4df0c55-791d-4a59-8363-9a89810262cc)


# FILTER TCP:
![image](https://github.com/user-attachments/assets/7bded20a-1f3c-4295-8043-439e60d2ff5b)


# APPLY RELAVANT FILTERS TCP.PORT=443
![image](https://github.com/user-attachments/assets/5aa45156-e298-4b3e-8a32-beee011c247f)

![image](https://github.com/user-attachments/assets/b0da2350-7d59-4269-86ac-ad7d5703a0bd)

![image](https://github.com/user-attachments/assets/ff54d05f-e34a-471f-8b48-44f95bf74d8c)

# DNS :

![image](https://github.com/user-attachments/assets/7d467cb6-077e-4e6f-9dd1-d708f0281972)


# Locate email data

Look for SMTP packets to see sender/receiver email addresses. Use "Follow TCP Stream" to view the full email headers and body if unencrypted.

# Extract Email Header Fields Analyze From, To, Subject, Date, Message-ID, and relay servers used in sending the email.
Perform activities like opening a website or sending an email through a client (e.g., Gmail via browser or Thunderbird).
![image](https://github.com/user-attachments/assets/1a2e75be-f75b-4c55-b980-c0e42f2ca892)

Stop the capture once done.

## RESULT:
Web browser artifacts and email headers were successfully analyzed using Wireshark

