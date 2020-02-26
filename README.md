# sonarqube-postgres-docker-compose

pleas follow

sudo sysctl -w vm.max_map_count=262144

sudo sysctl -w fs.file-max=65536

sudo ulimit -n 65536

sudo ulimit -u 4096
  
sudo mkdir sonarqube_conf sonarqube_data sonarqube_extensions sonarqube_bundled-plugins 

sudo chown "$USER":"$USER" sonarqube_conf sonarqube_data sonarqube_extensions sonarqube_bundled-plugins 

sudo chmod 777 sonarqube_conf sonarqube_data sonarqube_extensions sonarqube_bundled-plugins

sudo docker-compose  up -d --build

