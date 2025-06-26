# ElevateIntern_Project_1
Keylogger with Encrypted Data Exfiltration

Overview:
A proof-of-concept (PoC) keylogger built for ethical learning and demonstration. 
It Captures keystrokes using pynput. Encrypts each keystroke using cryptography (AES/Fernet).
Saves the encrypted logs with timestamps. Includes a separate decryption script.

Tools Used:
Python 3
pynput
cryptography

How to Run Key-logger:
1. Install Dependencies in the same folder as keylogger.py
   pip install -r requirements.txt

2. Run the Keylogger in your terminal (inside the keylogger/ folder):
   python keylogger.py

3. You’ll see:
   Keylogger started. Logs are encrypted.

Now type a few random keys in any application (like Notepad, browser, or even in the terminal window itself). It will keep running in the background and logging every keystroke.

4. Check the Encrypted Log File
   Go to:
   keylogger/logs/encrypted_log.txt
   Each line is encrypted, something like: (gAAAAABkzS0...etc...). You won't see the original keys in plain text — that's the purpose of Fernet encryption.

   
5. To decrypt the logs:
   python decrypt_logs.py

   You should now see all previously logged keystrokes printed clearly with timestamps.
   Example output:
   [2025-06-26 23:20:01] h
   [2025-06-26 23:20:02] e
   [2025-06-26 23:20:03] l
   [2025-06-26 23:20:04] l
   [2025-06-26 23:20:05] o

All Screenshots attached for refrence.


This projects are built for educational purposes only. 
Do not use any part of this code on real systems or websites without proper authorization. 
Unauthorized keylogging or vulnerability scanning may be illegal.
