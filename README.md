# Creating Vagrant Boxes for Custom Providers

Vagrant providers each require a custom provider-specific box format.

To turn this into a box:

    tar cvzf precise64-aws.box ./metadata.json ./Vagrantfile

This box works by using Vagrant's built-in Vagrantfile merging to setup
defaults for a custom cloud provider. These defaults can easily be
overwritten by higher-level Vagrantfiles (such as project root
Vagrantfiles).
