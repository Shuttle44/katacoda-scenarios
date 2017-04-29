Now we need to configure a few things.

## Task

First, let's prepare openssl:
`./config --shared`{{execute}}
The "--shared" parameters allows us to use the created files.

Second, compile it:
`make`{{execute}}

Now we need to copy 2 files:
`cp libssl.so /lib64`{{execute}}
`cp libcrypto.so /lib64`{{execute}}

Now let's look into this directory:
`cd /lib64`{{execute}}
`ls -l`{{execute}}

You should notice three things:
1. The libssl.so you just copied
2. There is a dynamic link, named libssl.so.10
3. This dynamic link points to a file named libssl.so.1.0.1e

Same applies to libcrypt.

Confusing? No worries, we'll solve this in the next step.