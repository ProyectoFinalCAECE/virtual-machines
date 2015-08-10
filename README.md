# virtual-machines
project virtual environments

Files
-----

Vagrantfile is a main Vagrant configuration. Typically it is supposed to be placed at the root of your project. Just put it whenever you want your box root should be.

Cheffile describes sources of cookbooks we use to provision packages demanded. It's used by Librarian to download all the cookbooks you need including referenced dependencies. Unless you already have it install it using 'gem install librarian-chef command'.


Ruby
----

In order to move forward we need to install Ruby:

1) install Ruby Version Manager: go to https://rvm.io/rvm/install and install the stable version.<br />
2) install Ruby 2.2.2: rvm install 2.2.2<br />
3) set default: rvm use 2.2.2 --default<br />
4) check: ruby --version


To finalize the setup and run your box you should:
--------------------------------------------------

1) put both of files to the root of your project (it will be the root of a virtual box).<br />
2) run 'librarian-chef install' to grab required cookbooks.<br />
3) run 'vagrant up' to download, provision and start your brand new box environment.<br />
4) run 'vagrant ssh' to sign in into the vm.

Vagrant
-------

https://docs.vagrantup.com/v2/

http://docs.vagrantup.com/v2/synced-folders/
