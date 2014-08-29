youtube-upload-shell-script
===========================

Shell script to automate the python youtube upload libary.

I run this in a Debian AWS instance to more quickly publish files to youtube. 
See blog post here: http://www.solonode.com/2014/08/upload-video-amazon-ec2-youtube-fast

This is handy because I often need to upload a number of videos from the same event (different presenters at a conference for example) and I want to be able to set some of the variables in a batch.

Current workflow is to upload the files to an Amazon S3 bucket, then sync this across to my AWS instance using the "sync-from-s2.sh" script.

So far, this approach appears to be 4-5x faster than uploading via Google Chrome.
