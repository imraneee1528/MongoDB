# Now Mongo DB Setup:

  sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 656408E390CFB1F5
 
# For ubuntu 20.04

  sudo sh -c 'echo "deb [ arch=amd64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/4.4 multiverse" > /etc/apt/sources.list.d/mongodb.list'
  # Now update repository 

  sudo apt-get update

# Install Mongodb Server:

  sudo apt -y install mongodb-org=4.4.1 mongodb-org-server=4.4.1 mongodb-org-shell=4.4.1 mongodb-org-mongos=4.4.1 mongodb-org-tools=4.4.1
 
  sudo systemctl enable mongod.service

  sudo systemctl start mongod.service

  sudo netstat -ntlp
