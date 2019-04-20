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
    python3 nwam.py [-h] [-o options] [-c count] [--about] key

    positional arguments:
      key         Your Shodan API key

    optional arguments:
      -h, --help  show this help message and exit
      -o options  Your Shodan query options (example: "city:\"Chicago\"")
      -c count    Amount of threads to use for mapping
      --about     About NWAM
      
### Attention
**THIS SCRIPT WILL SPREAD YOUR IP ON THE LOGS OF EVERY SINGLE CAMERA**  
Don't use it for accessing other people's cameras without permission, or you will probably get in trouble.
