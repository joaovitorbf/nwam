      _   ___          __     __  __ 
     | \ | \ \        / /\   |  \/  |
     |  \| |\ \  /\  / /  \  | \  / |
     | . ` | \ \/  \/ / /\ \ | |\/| |
     | |\  |  \  /\  / ____ \| |  | |
     |_| \_|   \/  \/_/    \_\_|  |_|
          Netwave Admin Mapper
    ~Why didn't you change the password?~
A tool that searches Shodan for Netwave IP cameras with default admin passwords.  
You aren't going to use it for anything bad... right?

It runs on Python 3 and it requires a Shodan API key which you can get for free by creating an account at [Shodan's website](https://www.shodan.io/).

#### Installation
    $ git clone https://github.com/joaovitorbf/nwam.git
    cd ./nwam
    pip install -r requirements.txt
  
#### Usage
    nwam.py [-h] [-q options] [-c count] [-o file] [--out-failed file]
            [--silent] [--iponly] [--about]
            key
    positional arguments:
      key                Your Shodan API key

    optional arguments:
      -h, --help         show this help message and exit
      -q options         Your Shodan query options (example: "city:\"Chicago\"")
      -c count           Amount of threads to use for mapping (default: 10)
      -o file            Output vulnerable IPs to file
      --out-failed file  Output IPs that failed to login to file
      --silent           Silence all stdout output
      --iponly           Output only vulnerable IPs to stdout
      --about            About NWAM
      
### Attention
**THIS SCRIPT WILL SPREAD YOUR IP ALL OVER THE LOGS OF EVERY SINGLE CAMERA**  
Don't use it for accessing other people's cameras without permission, or you will probably get in trouble.
