A quick and dirty JSON template to build the latest Debian Stretch 9.2.1

Note the handcoded MD5 and netinst ISO links.

```shell
validate debian-current-stable-vagrant.json
make
```

Add the box like so:
```shell
vagrant box add debian-stable-base ./debian-current-stable-vagrant.box
```
