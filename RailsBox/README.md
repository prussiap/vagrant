###Here you get my rails Vagrantfile and a link to the box.###

If you have never used vagrant you will need to follow the instuctions on the [site](http://docs-v1.vagrantup.com/v1/docs/getting-started/). In essence you need to download virtualbox and vagrant


##To install my railsbox:

1. Create a new director `mkdir myproject`
2. cd into myproject `cd myproject/`
3. Grab the Vagrantfile from here.
4. [Download the precise64rails.box](https://www.dropbox.com/s/bhxhp2vape52p0h/precise64rails.box) and add it `vagrant box add precise64rails.box precise64rails.box`
5. Run your dev environment `vagrant up`
6. `vagrant ssh` to get into your box. 
and you're ready to go now 


__note__: You may get prompted for which network adapter you are using on booting. Also once you ssh in your local files (aka the ones in the folder you vagrant up'd from) are available from the virtual machine by `cd /vagrant/`
This permits you to use your favorite IDE's or Vim on your local machine and to test your code from your vagrant box. 

Default port 3000 for rails is openned. 

To destroy your environment (this completely kills it) `vagrant destroy` or to suspend `vagrant suspend`
See vagrant documentation for the rest. 

##In the Box##
Versions of the files are below
* ruby 1.9.3
* rails 3.2.13
* bundle 1.3.5
* rvm 1.20.13
* sqlite3 3.7.9
* mysql 5.5.31
* postgres 9.1.9


