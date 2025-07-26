# Fixing-APT-issues-on-Kali-Linux
While I was updating my Kali Linux, I had a message: <br>

<img width="652" height="184" alt="Screenshot 2025-07-25 231553" src="https://github.com/user-attachments/assets/9b93304a-f5cd-40b2-88ee-f7ebc1dcc969" />

### What is the problem here?
This happened when the sources.list file pf my system was empty. This is cruicial because this file is what tells the APT where to look for the packages to install and update.

### How do we fix it?

1. Firstly open the file in a text editor as you prefer, I'll use nano: <br>

    ```bash
   sudo nano /etc/apt/sources.list

2. Now the text editor is open add the rolling repository:<br>

   ```bash
   deb http://http.kali.org/kali kali-rolling main contrib non-free non-free-firmware

3. After that save and exit the text editor by:

   - `CTRL + O`, then hit `Enter` to save  
   - `CTRL + X` to exit

4. Run the command:

   ```bash
   sudo apt update
 
### Right now you should be able to fetch updates and install new packages as it should.

For official documentation, visit <a heref="https://www.kali.org/docs/general-use/kali-linux-sources-list-repositories/">Kali Linux Sources</a>


`#cybersecurity` `#linux` `#kalilinux` `#bugfix` `#APT` `#troubleshooting` `#ethicalhacking`
