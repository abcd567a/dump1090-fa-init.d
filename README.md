# dump1090-fa-init.d

## For OS with SysVinit, but without systemd

### STEP 1 - Download init file for dump1090-fa</br>
```
sudo wget -O /etc/init.d/dump1090-fa https://github.com/abcd567a/dump1090-fa-init.d/raw/main/dump1090-fa    

```

### STEP 2 - Initialize for automatic start at boot </br> 
```
sudo chmod +x /etc/init.d/dump1090-fa 
```
```
sudo update-rc.d dump1090-fa defaults 
```
```
sudo /etc/init.d/dump1090-fa start 

```


### USAGE - Start/Stop/Restart </br>


```
sudo service dump1090-fa start  
```
```
sudo service dump1090-fa stop  
```
```
sudo service dump1090-fa restart  

```

### USAGE - Status & Log </br>
```
sudo service dump1090-fa status 
```
```
cat /var/log/dump1090-fa.log  

```

