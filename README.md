## Extract Binary

### strings
Look for strings in the binary:

    strings filename
    
still gibberish, possible compressed or encrypted.

### binwalk

    wget https://github.com/devttys0/binwalk/archive/master.zip
    unzip master.zip
    (cd binwalk-master && sudo python setup.py uninstall && sudo python setup.py install)

[install](https://github.com/ReFirmLabs/binwalk/wiki/Quick-Start-Guide)

File Info:

    binwalk filename
    
Extract:

    binwalk -e filename