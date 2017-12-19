## Extract Binary

### strings
Look for strings in the binary:

    strings filename
    
still gibberish, possibly compressed or encrypted try binwalk.

### binwalk
Install:

    wget https://github.com/devttys0/binwalk/archive/master.zip
    unzip master.zip
    (cd binwalk-master && sudo python setup.py uninstall && sudo python setup.py install)

For Extracting:

    sudo ./binwalk-master/deps.sh

[Offical Quick Start](https://github.com/ReFirmLabs/binwalk/wiki/Quick-Start-Guide)

File Info:

    binwalk filename
    
Extract:

    binwalk -e filename
    
Remove install files:

    rm master.zip
    sudo rm binwalk-master -fr