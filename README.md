# Title me

Describe me.

## EC2 UserData

This section describs what will be expected to be in the UserData at boot time.

- `HOSTNAME`

# Instal Packer

The image is managed and created by [Packer](https://www.packer.io/intro/getting-started/install.html) by HashiCorp. This means you have to install their tool first.

# Then build the AMI

The image can be build via the following command:

``` sh
packer build -var-file=vars.json main.json
```

# Overriding variables

Variables in vars.json can be overridden like so:

``` sh
packer build -var-file=vars.json -var region=us-east-2 main.json
```

# Troubleshooting

Explain how to troubble shoot the AMI.