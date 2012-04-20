Disclaimer: This is one of the first things I've written in Python. So be gentle. Recovering Rubyist here :)

```bash
    $ domainr talsafran
    Looking up domains for talsafran...
        talsafran.com - taken
        talsafran.net - available [1]
        talsafran.org - available [2]
        talsafr.an - available [3]
        talsa.fr - available [4]
        tals.af - available [5]
        tal.sa - available [6]
        ta.ls - unavailable
        tls.fr - taken
        t.al - unavailable
        t.ls - unavailable
        tl - tld
```

## Domainr Command Line Interface
If you're like me, you love the website [Domai.nr](http://domai.nr). You type in a name you have in mind for a domain and it spits back as many clever domain possibilities as it can find, including domain hacks. That's badass.

Now if you're *really* like me, you like doing things in the command line as much as possible. I check for domains every time a silly idea pops into my head, which is very often. And I like doing it fast. So that's why I wrote this Domainr CLI.

## Requirements and Installation
First go and grab the repo:

```bash
    $ git clone https://github.com/talsafran/domainr.git
```

I'm fairly confident you need version 2.6 or greater for the json library. So go and get that.

Now you can either copy the script into your PATH or create a symlink. Whatever floats your boat.

```bash
    $ cp domainr /usr/local/bin
```

## How to use this thing
Very simple. Just type in ``domainr`` and the name of the site you're looking for.

```bash
    $ domainr talsafran
    Looking up domains for talsafran...
        talsafran.com - taken
        talsafran.net - available [1]
        talsafran.org - available [2]
        talsafr.an - available [3]
        talsa.fr - available [4]
        tals.af - available [5]
        tal.sa - available [6]
        ta.ls - unavailable
        tls.fr - taken
        t.al - unavailable
        t.ls - unavailable
        tl - tld
```

It even works with multiple domains.

```bash
    $ domainr talsafran sharonsafran
    Looking up domains for talsafran...
        talsafran.com - taken
        talsafran.net - available [1]
        talsafran.org - available [2]
        talsafr.an - available [3]
        talsa.fr - available [4]
        tals.af - available [5]
        tal.sa - available [6]
        ta.ls - unavailable
        tls.fr - taken
        t.al - unavailable
        t.ls - unavailable
        tl - tld
    Looking up domains for sharonsafran...
        sharonsafran.com - available [7]
        sharonsafran.net - available [8]
        sharonsafran.org - available [9]
        sharonsafr.an - available [10]
        sharonsa.fr - available [11]
        sharons.af - available [12]
        sharon.sa - available [13]
        sha.ro - available [14]
        shrns.fr - available [15]
        shar.nsafr.an - available [16]
        shar.nsa.fr - taken
        shar.ns.af - taken
        shar.n.sa - available [17]
        sh.ar - unavailable
        s.hr - available [18]
        sh - tld
```

And, you can even register a domain from the CLI. All you have to do is pass in the number associated with the **available** domain. So, you'd be running something like:

```bash

    $ domainr register 3

```

Will bring up a new tab in your default browser (if the domain is available), to register the domain!

-- [@talsafran](http://twitter.com/talsafran)
