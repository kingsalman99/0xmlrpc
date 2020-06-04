# 0xmlrpc
mass xmlrpc vulnerability findng and auto report sending 

# Requirments for email notification

```
$ sudo apt install ssmtp
$ sudo apt install mailutils
```

Note: I am using mailx to send the mail

Make sure you have configured your ssmtp.config file Edit /etc/ssmtp/ssmtp.conf and add those configs


```
UseSTARTTLS=YES
FromLineOverride=YES
root=yourname@gmail.com
mailhub=smtp.gmail.com:587
AuthUser=yourname@gmail.com
AuthPass=YourEmailPassword
```

# Usage

```
$ 0xmlrpc urls.txt yourname@gmail.com
```
