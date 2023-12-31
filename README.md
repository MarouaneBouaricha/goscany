# GoScany

Simple port scanner CLI written Go,
a try of implementing the native concurrency mechanism in the Go Language.

## Requirements
```
go 1.13 or later
clir v1.0.4
```

## Installing
### brew
```shell
brew tap MarouaneBouaricha/releases
```
```shell
brew install goscany
```
### linux
from binay releases
```
wget https://github.com/MarouaneBouaricha/goscany/releases/tag/v0.0.5/goscany_0.0.5_linux_amd64.tar.gz
```
```
tar -xcf goscany_0.0.5_linux_amd64.tar.gz
```
```
sudo mv goscany_0.0.5_linux_amd64.tar.gz /usr/local/bin/goscany
```
```
sudo chmod +x /usr/local/bin/goscany
```

## Usage
```
gscany v0.0.1 - Fast Port Scanner CLI

Available commands:

   basic   Scan for well known ports (1-1024)
   wide    Scan for all ports

Flags:

  -help
        Get help on the 'gscany' command.

```


## Example Usage

```
goscany wide -host 192.168.1.6 -n 2500 -p tcp

```

### output:

```
Scanning...
 80 [Open] -> http 
 135 [Open] -> UNKNOWN  
 139 [Open] -> netbios  
 443 [Open] -> https    
 445 [Open] -> Samba    
 1536 [Open] -> UNKNOWN 
 1537 [Open] -> UNKNOWN 
 1538 [Open] -> UNKNOWN 
 1539 [Open] -> UNKNOWN 
 1540 [Open] -> UNKNOWN 
 1541 [Open] -> UNKNOWN 
 3306 [Open] -> MySQL   
 5040 [Open] -> UNKNOWN 
 5357 [Open] -> UNKNOWN 

Finished in  54.6971717s

```
