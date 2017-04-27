Now we edit the links so that our files get used.

## Task

First, we delete the dynamic link libssl.so.10:
`rm libssl.so.10`{{execute}}

Next, we create a new dynamic link, which has the same name, but points to our file:
`ln -s libssl.so libssl.so.10`{{execute}}

We do the same with the libcryt.so.10. First, remove old link:
`rm libcrypt.so.10`{{execute}}

Next, create a new dynamic link:
`ln -s libcrypt.so libcrypt.so.10`{{execute}}

Let's see what we did:
`ls -l`{{execute}}

As you can see, our files are now linked and will be used.