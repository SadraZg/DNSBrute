# DNSBrute
Using this tool you only pass your target Domain name and a DNS wordlist, and as a result you will get a complete list of fresh subdomains of your target

### Prerequisites
Python 3.6+ 

[DNSGen](https://github.com/ProjectAnte/dnsgen)

[ShuffleDNS](https://github.com/projectdiscovery/shuffledns)

[Anew](https://github.com/tomnomnom/anew)

Good DNS wordlist 

Fresh Resolver List (You can get it using [this](https://github.com/BonJarber/fresh-resolvers))

### How to use?
Usage: dnsbrute.py [options]

#### Options:
-h, --help  show this help message and exit

-d DOMAIN, --domain=DOMAIN
     Enter your target domain name.

-w WORDLIST, --wordlist=WORDLIST
     Enter your DNS wordlist.

-r RESOLVERS, --resolvers=RESOLVERS
     Enter your resolvers filename.

-f FAST, --fast=FAST
     Do you want to create shorter wordlist from DNSGen (y/n)? [Default: y]

### Examples
python3.8 dnsbrute.py -d target.tld -w dns_wordlist.txt

python3.8 dnsbrute.py -d target.tld -w dns_wordlist.txt -f n
