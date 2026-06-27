
1. What Is SSH?
	- SSH(secure Shell ) it is help us login and manage data btw git & github without asking username and password always to make changes 
	- like opening phone with fingerprint and login mail account with passkeys 
	- key pairs - Private Keys :Stays on your computer .Never share it
	- Public key - Uploaded to GitHub 
2. Why use SSH instead of HTTPS ?
	- Uses username /password or Personal Access Token {PAT}
	- Need to enter password frequently 
	- Cryptographic keys
	- No password after passkey generated 
	- Faster GIt operations 
	- Manly for developers 
3. Prerequisties 
	- git --version
	- username # git config --global user.name "Your Name"
	- email # git config --global user.email "your@email.com"
	- verify # git config --global --list 
	-  version # ssh -V
	- generate of ssh key # ssh-keygen -t ed25519 -C "harshith@gmail.com"
	- for older ssh  # ssh-keygen -t rsa -b 4096 -C "your@email.com"
	- after enter skip or enter again 
	- for linux  ,  ~/.ssh/id_ed25519 , ~/.ssh/id_ed25519.pub
	- for windows C:\Users\Username\.ssh\
4. Start ssh agent
     - for linux eval "$(ssh-agent -s)"
     - for powershell Start-Service ssh-agent
5.  Add ssh key 
	- ssh-add ~/.ssh/id_ed25519
6.  Copy Public key
	- cat ~/.ssh/id_ed25519.pub
7. Test Connection
	- ssh -T git@github.com
	- Are you sure you want to continue connecting?
	- Hi username! ,
	- You've successfully authenticated...
8. change existing repo from HTTPS to SSH
	- git remote -v
	-  to remove # git remote set-url origin git@github.com:username/repository.git
9. FAQ
	**Q. Can I use different SSH keys for different GitHub accounts?**  
	Yes. Configure multiple SSH keys using an SSH config file.

	**Q. Do I need to generate a new key for every repository?**  
	No. One key per device is usually enough.

	**Q. What is the difference between the public and private key?**  
	The **public key** is shared with GitHub. The **private key** stays on your computer and must never be shared.

	**Q. Is SSH available on both Windows and Linux?**  
	Yes. The commands are almost identical, with only minor differences in file locations and how the SSH agent is started.