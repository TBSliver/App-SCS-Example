# Example App-SCS Site

This is an example site written using App-SCS. to run, perform the following:

```
mkdir site
cd site
git clone git://git.shadowcat.co.uk/scpubgit/App-SCS.git
cd App-SCS
cpanm --installdeps . # assuming you have a local lib set up
cd ..
git clone git@github.com:TBSliver/App-SCS-Example.git
cd App-SCS-Example
./bin/site server
```

Then you can connect to the Server on localhost:5000

# Full Installation

You will need the following things installed before you start:

- curl
- build-essential (or equivalent on non-debian distros) 

```
echo '[ $SHLVL -eq 1 ] && eval "$(perl -I$HOME/perl5/lib/perl5 -Mlocal::lib)"' >> ~/.bashrc # or equivalent file

curl -L https://cpanmin.us | perl - --local-lib=~/perl5 local::lib App::cpanminus

mkdir Site-Generation
cd Site-Generation

git clone git://git.shadowcat.co.uk/scpubgit/App-SCS.git
cd App-SCS

cpanm --installdeps .
cpanm Starman # optional dependency
cd ..

git clone https://github.com/TBSliver/App-SCS-Blog.git

git clone git@github.com:TBSliver/App-SCS-Example.git
cd App-SCS-Example
./bin/site server
```

There will now be a test server running on *:5000
