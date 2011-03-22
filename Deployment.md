# Deployment

  * Capistrano

  * [Sprinkle](http://github.com/crafterm/sprinkle) is a software provisioning
    tool you can use to build remote servers with. eg. to install a Rails, or
    Sinatra stack on a brand new slice directly after its been created

    [Collection of recipes for various Ruby on Rails deployment setups](http://github.com/karmi/rails-deployment-setups-sprinkle)

## Cloud

### AWS EC2

  * [Fog](http://github.com/geemus/fog) is the Ruby cloud computing library.
  * [Judo](http://github.com/mipearson/judo)
  * [Sumo](http://github.com/adamwiggins/sumo), [Sumo: One-off EC2 Instance Launching](http://adam.heroku.com/past/2009/8/28/sumo_oneoff_ec2_instance_lanching/)

  * [MongoDB on EC2 and EBS](http://www.slideshare.net/jrosoff/mongodb-on-ec2-and-ebs)

#### PoolParty.rb

PoolParty.rb uses Chef to deploy to Amazon's EC2 cloud service and supports auto-scaling.

 * [PoolParty.rb](https://github.com/auser/poolparty) ([Website](http://auser.github.com/poolparty/index.html))

 * [VMware (Fusion) and PoolParty setup](http://auser.github.com/poolparty/vmware_setup.html)

#### Rubber

Rubber is a Capistrano plug-in to deploy to Amazon's EC2 cloud service.

  * [Rubber](https://github.com/wr0ngway/rubber)

  * [How to Deploy a Rails app to EC2 in less than an hour using Rubber](http://ginzametrics.com/deploy-rails-app-to-ec2-with-rubber.html)


### AWS Elastic Beanstalk

  * [AWS Elastic Beanstalk](http://aws.amazon.com/elasticbeanstalk/)

  * [JRuby on Rails on AWS Elastic Beanstalk](http://blog.headius.com/2011/01/jruby-on-rails-on-amazon-elastic.html)

## Virtual Machines

#### Vagrant

Vagrant uses Chef or Puppet to deploy to virtual machines using [VirtualBox](http://www.virtualbox.org/).

  * [Vagrant](http://vagrantup.com/)

  * [Creating a Local Riak Cluster with Vagrant and Chef](http://blog.basho.com/2011/02/04/creating-a-local-riak-cluster-with-vagrant-and-chef/)

  * [Making CI easier to do than not to with Hudson CI and Vagrant](http://drnicwilliams.com/2010/11/09/making-ci-easier-to-do-than-not-to-with-hudson-ci-and-vagrant/)

  * [Testing Rails for the masses!](http://blog.cookiestack.com/post/571168451/testing-rails-for-the-masses)

  * [Vagrant VBox for Jenkins](https://github.com/abtris/vagrant-hudson)

  * [Using Vagrant with the Opscode Platform](http://wiki.opscode.com/display/chef/Vagrant)

  * [VeeWee](https://github.com/jedi4ever/veewee) eases the building of Vagrant boxes
