# Web Honeypot
(Antisyphon training lab from Cyber Deception/Active Defense)<br><br>
Full lab explanation available on my <a href="https://medium.com/@swathitadepalli/active-defense-and-cyber-deception-antisyphon-training-44c0ee851be4#b4e2">Medium</a>
## Honeypot
- Navigate to the honeypot directory: ```cd /opt/owa-honeypot/```
- Start the honeypot
<pre>sudo python3 owa_pot.py</pre>
- In another terminal window, grab your IP and print the last 10 lines of  ```dumpass.log```
<pre>ifconfig</pre>
<pre>tail -f dumpass.log</pre>
<img width="647" alt="Screenshot 2025-03-30 at 10 23 56 PM" src="https://github.com/user-attachments/assets/80d93f0f-4945-475d-be38-3cfad32b8153" /><br><br>
- Access the honeypot via the following URL: ```http://{YOUR LINUX IP}```<br><br>
<img width="500" alt="Screenshot 2025-03-30 at 10 28 22 PM" src="https://github.com/user-attachments/assets/aac67f80-7e54-4b35-8506-bc7d6128208b" /><br><br>
- Try several usernames and passwords. The login attempts will be recorded in the log:<br><br>
 <img width="639" alt="Screenshot 2025-03-30 at 10 30 29 PM" src="https://github.com/user-attachments/assets/806b9ec6-c202-4b70-8f23-479388246531" /><br><br>
 ## OWASP ZAP
 - Now, let's run an automated scan using OWASP ZAP:<br><br>
<img width="643" alt="Screenshot 2025-03-30 at 10 37 14 PM" src="https://github.com/user-attachments/assets/e016051c-bdbd-471e-8f44-87b33e5aa201" /><br><br>
<img width="936" alt="Screenshot 2025-03-30 at 10 40 10 PM" src="https://github.com/user-attachments/assets/1a419b5d-2b11-4efa-9462-f34948efe724" /><br><br>
- Attack strings should now appear in your logs:
<img width="640" alt="Screenshot 2025-03-30 at 10 44 16 PM" src="https://github.com/user-attachments/assets/22acc00a-e4b2-46a2-9ce1-84684b5aab90" /><br><br>
<a href="https://github.com/swathinator/Homelabs">Back to Homelabs</a>
