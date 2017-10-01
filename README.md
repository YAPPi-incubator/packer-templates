Get a copy of [packer](https://packer.io/) for your platform.

Build AMI
```
# get submodules
$ git submodule init                                                                        
$ git submodule update

# configure AWS access key
$ cp .env.example .env
# fill your details in the .env file

$ packer build -var-file=jenkins.json builders/ami.json
```

