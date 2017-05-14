We're nearly done, this is the last step.

## Task

Everything is ready. We installed an Apache, set up the ability to use HTTPS-Connections
and made sure that the files from a vulnerable version of openssl will be used.

So let's get the server running:
`service httpd start`{{execute}}

On your second terminal, install wget and download the following:
https://gist.githubusercontent.com/eelsivart/10174134/raw/8aea10b2f0f6842ccff97ee921a836cf05cd7530/heartbleed.py

That is all. Happy Hacking!