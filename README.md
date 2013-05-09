scpc
====

**compress here - do scp - uncompress there**

The `scp` command when used recursively each file will be sent on a new connection - which is very slow when uploading multiple files.

`scpc` does the same but, it compresses the source directories in local before secure copying to the destination. 
It automatically uncompresses the file to specified target remote directory. This saves bandwidth and reduces time taken to upload.

Usage
-----

    $ scpc folder1 folder2 abhinay@abhiomkar.in:/home/abhinay/www/
