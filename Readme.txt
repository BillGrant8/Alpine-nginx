Within installation directory:

vagrant up

goto 192.168.50.100:8080

Vagrant ssh (to get into the VM)  
# Then add gem install for specserv to the VM (high risk issues creating a Ruby Shim for my OSX under current circumstances) 

SpecServ
bundle exec rspec spec/Dockerfile_spec.rb

    1  sudo apt-add-repository ppa:brightbox/ruby-ng
    2  sudo apt-get update
    3  sudo apt-get install ruby2.4
    4  sudo gem install serverspec
    5  serverspec-init 
   16  touch gemfile
   17  mv gemfile Gemfile
   19  nano Gemfile 
   21  bundle --v
   22  sudo gem install bundler
   23  bundle install 
   24  mkdir spec
   30  sudo gem install docker-api
   41  docker ps
   42  wget localhost:80
   43  wget localhost:8080 
   59  ps -ef |pgrep nginx

bundle exec rspec spec/Dockerfile_spec.rb


Curl 192.168.50.100:8080



