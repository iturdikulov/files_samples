Just files samples.

To set associations, if needed - I just use nautilus.
Right click on file -> properties -> open with -> select app -> set default

To quickly setup associations (Linux distro with `perl-file-mimeinfo` installed) you can use this one-liner script:
```
# cd to file_sampls projects first
# select program which will be used to open this file type 
# and then close opened program to setup next mime type

for f in ./*.*; do echo "set association to $f"; mimeopen -d "$f"; done
```

Or check _assoc_sample.sh script
