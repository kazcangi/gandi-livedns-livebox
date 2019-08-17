# gandi-livedns-livebox
Update a record in your Gandi's domain with your Livebox public IP

You need to install [lbws](https://github.com/kazcangi/lbws)

## Install

Copy gandi-livedns-livebox to a directory, and lbws in the same directory

Create a sample config file with :

```
./gandi-livedns-livebox > gandi-livedns-livebox.ini
```
Edit it and save. Then just launch with ```./gandi-livedns-livebox```

## Usage

```
usage: gandi-livedns-livebox [-h] [-V]
                             [-L {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
                             [-R | -C | -D | -I]

Update Gandi DNS with current public IP. Need a config file in the same
directory named gandi-livedns-livebox.ini

optional arguments:
  -h, --help            show this help message and exit
  -V, --version         show program's version number and exit
  -L {DEBUG,INFO,WARNING,ERROR,CRITICAL}, --log {DEBUG,INFO,WARNING,ERROR,CRITICAL}
                        Change logging level, default INFO
  -R, --logrotatefile   Print logrotate file example, can be redirected to a
                        file
  -C, --sampleconfig    Print sample config file, can be redirected to a file
  -D, --dnsip           Get current IP registered in DNS
  -I, --currentip       Get current public IP
  
