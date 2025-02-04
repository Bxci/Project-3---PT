# Project-3---PT


1️⃣ User Verification
The script checks if the user is running it as root. If not, it exits.

2️⃣ Directory Setup
The user is asked to enter a directory name where all results will be stored.
If the directory does not exist, it is created.

3️⃣ Password List Handling
The script asks the user if they want to use a built-in password list or a custom one for brute-force attacks.
If using the built-in list, it downloads user_pass.txt from GitHub.

4️⃣ Scan Selection (Basic or Full)
The user can choose between:
Basic Scan

Runs nmap scans for service and vulnerability detection.
Uses masscan for UDP scanning.
Saves results in text files.
Full Scan

Performs a deep nmap vulnerability scan.
Runs brute-force attacks using medusa (for SSH, Telnet, FTP, RDP).
Extracts CVE identifiers from the scan results.
Uses searchsploit to find known exploits for detected CVEs.

5️⃣ Post-Scan Options
The user can:
List the scan results (ls command).
Search inside the generated reports using grep.
Zip all the results for storage.

6️⃣ User Interaction
The script asks the user multiple questions before running operations (e.g., "Do you want to continue?", "Enter an IP address", etc.).
If the user chooses to proceed, the script executes the requested operations.

7️⃣ Error Handling
The script checks if the user enters an invalid IP format and exits if incorrect.
It prevents execution if the user is not root.
