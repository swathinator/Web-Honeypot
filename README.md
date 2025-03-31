# Web-Honeypot
(Antisyphon training lab from Cyber Deception/Active Defense)
## Honeypot
-  Navigate to ```cd /opt/owa-honeypot/```
- Start the honeypot
<pre>sudo python3 owa_pot.py</pre>
- In another window, grab your IP and print the last 10 lines of ```dumpass.log```
<pre>ifconfig</pre>
<pre>tail -f dumpass.log</pre>
<img width="647" alt="Screenshot 2025-03-30 at 10 23 56 PM" src="https://github.com/user-attachments/assets/80d93f0f-4945-475d-be38-3cfad32b8153" /><br><br>
- Let's access the honeypot ```http://{YOUR LINUX IP}```<br>
<img width="500" alt="Screenshot 2025-03-30 at 10 28 22 PM" src="https://github.com/user-attachments/assets/aac67f80-7e54-4b35-8506-bc7d6128208b" /><br><br>

- Try several usernames and passwords, the attemps will be in the log:
 <img width="639" alt="Screenshot 2025-03-30 at 10 30 29 PM" src="https://github.com/user-attachments/assets/806b9ec6-c202-4b70-8f23-479388246531" /><br><br>
 - Let's run an automated scan using OWASP ZAP:<br><br>
<img width="643" alt="Screenshot 2025-03-30 at 10 37 14 PM" src="https://github.com/user-attachments/assets/e016051c-bdbd-471e-8f44-87b33e5aa201" /><br><br>
<img width="936" alt="Screenshot 2025-03-30 at 10 40 10 PM" src="https://github.com/user-attachments/assets/1a419b5d-2b11-4efa-9462-f34948efe724" /><br><br>
- Attack strings should appear in your logs:
<img width="640" alt="Screenshot 2025-03-30 at 10 44 16 PM" src="https://github.com/user-attachments/assets/22acc00a-e4b2-46a2-9ce1-84684b5aab90" />
