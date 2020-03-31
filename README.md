# Info
- Group 3 in Knowledge Representation and Reasoning Class - C214, UIT 2020.
- Lecturer: Miss Nguyễn Thị Ngọc Diễm
- Member:
  - Nguyễn Ôn Ngọc Bảo
  - Huỳnh Khánh Hoà
  - Lê Phạm Thiên Bằng
  - An Minh Hùng

# Introduction how to use Git - Updated at 09:13 PM, 31/03/2020 by @ngbao161199

## 1. Installation

### 1.1. For Window: 
- Go to this site and download: https://git-scm.com/

### 1.2. For Linux: 
- Use this command from Terminal:
```
sudo apt-add-repository ppa:git-core/ppa
sudo apt-get update
sudo apt-get install git
```

### 1.3. For Mac: 
- Rich kids! Google please :)

## 2. SSH Keys creation :)

### 2.1. For Window: 
- Find and Run Windows PowerShell as administrator.
- Run this command: 
```Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux```
- Restart your computer.
- Open GitBash by Right Click on the folder you're in, choose `Git Bash Here`.
- Run this command (Remember to use email that you use to register your Github account): 
```ssh-keygen -t rsa -C "your.email@address"```
- Then:
  - Type new file name or press Enter to accept default file name.
  - Press Enter if need no passphrase.
  - The key is created successfully after this step.
- Open your file name with Notepad++. If you choose default file name, it must be `id2_rsa.pub`.
- After opening the file, copy the whole content showed in the file (from ssh-rsa to youremail).
- Go to [this site](https://github.com/settings/keys)(Settings> SSH and GPG keys) in your Github Account. 
- Choose `New SSH Keys`, type anything in `Title` and paste everything inside your rsa file to `Key` field.
- Done.

### 2.2. For Linux - Update later

### 2.3. For Mac - Update later

## 3. Git Usage

### 3.1. git config
- This step is to declare your identification with your computer,... in your local environment. 
- Run this command from Git Bash:
```
git config --global user.name "Your Full Name"
git config --global user.email "your.email@mail.ext"
```

### 3.2. git clone

- **Note**: This step is to copy (download) all contents of an existing project in remote repository to your working directory. Please note that this step is only conducted when the your working directory does not have any content of that project.
- Right click at the folder you want the new repository to be downloaded
-	Open GitBash
-	Type the following command:
```git clone [project/url]```
- Example with our project:
```git clone git@github.com:ngbao161199/Knowledge-Representation-and-Reasoning-UIT.git```

### 3.3. git status

- **Note**: This step is to check status of git contents: updated or not (compared local with remote), files sent to server or not and where it is (still in working area, staging area, or in local) .
- Command: `git status`.

### 3.4. git pull
- This step is to update content from remote repository to local repository.  It means you already have that project in your local repository.
- Right click at the working directory you want to update files, open Git Bash & check this command:
```
git pull
```

### 3.5. git add, git commit, git push

- **Note**: These are the series of steps to upload contents from local repository to remote repository. 
- Check it:
>- Right click at the working directory you want to upload files
>- Open GitBash
>- If you want to upload all content of the folder into Staging Area, type the following command: `git add .`
>- If you want to upload 1 specific file into Staging Area, type the following command: `git add <filename>`
>- To add the files into Local Repository, type the following command: `git commit -m “commit message”`
>- To upload the files into Remote Repository, type the following command: `git push`


