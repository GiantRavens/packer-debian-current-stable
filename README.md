A quick and dirty JSON template to build the latest Debian

Make sure that Packer is installed

```shell
brew install vagrant packer
```

Note the handcoded MD5 and netinst ISO links.

```shell
validate debian-current-stable-vagrant.json
make
```

Add the box like so:

```shell
vagrant box add debian-stable-base ./debian-current-stable-vagrant.box --name debian-buster
```
