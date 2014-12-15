# Example App-SCS Site

This is an example site written using App-SCS. to run, perform the following:

```
mkdir site
cd site
git clone scpubgit@git.shadowcat.co.uk:App-SCS.git
cd App-SCS
cpanm --installdeps . # assuming you have a local lib set up
cd ..
git clone git@github.com:TBSliver/App-SCS-Example.git
cd App-SCS-Example
./bin/site server
```

Then you can connect to the Server on localhost:5000
