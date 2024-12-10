## What is this repo for?
This `repo` was created to house a `hosts` file to be used with [Pi-hole](https://github.com/pi-hole/pi-hole) to block pesky ads on the web accross all devices connected to your network.
This `repo` only came to be to remove some ads that were still making their way in past other host block lists I have.

## What is a hosts file?
A hosts file, named `hosts` (with no file extension), is a plain-text file used by all operating systems to map hostnames to IP addresses.

In most operating systems, the `hosts` file is preferential to `DNS`. Therefore if a domain name is resolved by the `hosts` file, the request never leaves your computer.

Having a smart hosts file goes a long way towards blocking malware, adware, and other irritants.

For example, to nullify requests to some doubleclick.net servers, adding these lines to your hosts file will do it:

```
# block doubleClick's servers
0.0.0.0 ad.ae.doubleclick.net
0.0.0.0 ad.ar.doubleclick.net
0.0.0.0 ad.at.doubleclick.net
0.0.0.0 ad.au.doubleclick.net
0.0.0.0 ad.be.doubleclick.net
# etc...
```

## How do I use your hosts file?
First copy the following URL
```
https://raw.githubusercontent.com/jcokell/Hosts/refs/heads/main/hosts
```
Go to your "Adlists" section on you Pi-hole dashboard and paste it into the "Address" box under "Add a new adlist"

And you're done! Pi-hole will automatically download and use an updated version of the `hosts` file whenever you update the Gravity (list of blocked domains)
