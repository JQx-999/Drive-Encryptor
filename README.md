# Drive-Encryptor
Encrypt your drive <br>
## Can only be used in Linux
<br>
Author: JQx
You are free to reproduce, contibute, change, modify this code.
Preparation:
Backup every thing from the target drive that you wanna encrypt. This code is designed to destroy the drive/partition. It has no warranty. YOU ARE AT YOUR OWN RISK. Make sure to unmount the drive before use. The script uses cryptsetup to encrypt using LUKS. This only works on linux. You will need specific packages to format to specific format. ext4: e2fsprogs, btrfs: btrfs-progs, fat32: dosfstools, ntfs: ntfs3. I recommend you using a safe 14 character password. But it's upto you cuz I myself use 4 digit password tbh. This code only automates the work. It is designed to make the drive accessible to everyone. You could change the permissions afterward. I made this code for my personal convinience, you may choose to use it. 
How to use it? :
This script will first ask about the partition. Suppose I want to encrypt sda2. So I will type "sda2" and nothing else. Then it will open the cryptsetup to encrypt the drive. Type "YES" as prompted. Choose a STRONG password for your drive. It will ask again for the passowrd to open the drive. Choose the specific file format if prompted. BACKUP the header file (Type Y to continue). Finished. Now disconnect the drive and reconnect the drive and use it as intended. <br>

Use the following code to use it.
```
git clone https://github.com/JQx-999/Drive-Encryptor.git
cd Drive-Encryptor/Encryptor && bash ./main
```
