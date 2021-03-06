
##  WEB ARCHITECTURE
- https://engineering.videoblocks.com/web-architecture-101-a3224e126947
- https://arcentry.com/blog/scaling-webapps-for-newbs-and-non-techies/
- https://github.com/sathishvj/awesome-gcp-certifications
- https://github.com/binhnguyennus/awesome-scalability
- https://github.com/bregman-arie/devops-exercises
- https://github.com/jdauphant/awesome-ansible

## TOOLS
- https://crontab.guru/
- https://cronitor.io/index
- https://certbot.eff.org/
- https://jmeter.apache.org/
- https://www.netdata.cloud/
- https://www.whatsmydns.net/
- https://www.cdn77.com/tls-test
- https://www.sslshopper.com/ssl-checker.html
- https://sshreach.me/
- https://ngrok.com/

## TOOLS OSS
- https://github.com/Qovery/engine
- https://github.com/loadimpact/k6
- https://github.com/kruize/kruize
- https://github.com/grafana/grafana
- https://github.com/caprover/caprover
- https://github.com/nicolargo/glances
- https://github.com/alexfernandez/loadtest
- https://github.com/ripienaar/free-for-dev
- https://github.com/ClementTsang/bottom
- https://github.com/earthly/earthly
- https://github.com/SigNoz/signoz
- https://github.com/six-ddc/plow

## VIM

- https://www.fprintf.net/vimCheatSheet.html

## SERVICES
- https://vercel.com/
- https://www.netlify.com/
- https://www.checklyhq.com/
- https://www.compose.com/

## KUBERNETES
- https://helm.sh/
- https://github.com/appvia/kev
- https://github.com/keel-hq/keel
- https://github.com/lensapp/lens
- https://github.com/kedacore/keda
- https://github.com/Portshift/kubei
- https://github.com/hobby-kube/guide
- https://github.com/godaddy/terminus
- https://github.com/porter-dev/porter
- https://github.com/stackrox/kube-linter
- https://github.com/cloudmelon/melonkube
- https://github.com/kubernetes/dashboard
- https://github.com/kubernetes/kubernetes
- https://github.com/eon01/kubernetes-workshop
- https://github.com/eldada/kubernetes-scripts
- https://github.com/kubernauts/jmeter-kubernetes
- https://github.com/tomhuang12/awesome-k8s-resources
- https://kubernetes.io/docs/tutorials/kubernetes-basics/
- https://github.com/kelseyhightower/kubernetes-the-hard-way

## REDIS
- https://github.com/JamzyWang/awesome-redis

## DOCKER
- https://github.com/qdm12/devtainr
- https://github.com/jesseduffield/lazydocker
- https://github.com/tomMoulard/make-my-server
- https://github.com/veggiemonk/awesome-docker
- https://github.com/buildkite/docker-puppeteer
- https://github.com/ufoscout/docker-compose-wait
- https://github.com/geerlingguy/ansible-role-docker    
- https://github.com/JeremyLikness/usda-microservice
- https://github.com/felixfbecker/semantic-release-docker
- https://labs.play-with-docker.com/
- https://youtu.be/3c-iBn73dDE Docker Tutorial for Beginners [Full Course in 3 Hours]
- https://dev.to/softchris/5-part-docker-series-beginner-to-master-3m1b
- https://dzone.com/articles/build-and-deploy-a-mongodb-angular-nodejs-app-usin

## DOCKER IMAGES
- https://github.com/bunkerity/bunkerized-nginx
- https://github.com/bunkerity/bunkerized-mariadb
- https://github.com/bunkerity/bunkerized-php

1) 𝐝𝐨𝐜𝐤𝐞𝐫 𝐭𝐨𝐩:  Displays the container's running processes
$ docker top <container>

2) 𝐝𝐨𝐜𝐤𝐞𝐫 𝐩𝐨𝐫𝐭: Lists container's port mappings
$ docker port <container>

3) 𝐝𝐨𝐜𝐤𝐞𝐫 𝐤𝐢𝐥𝐥: Kills the process! (not ideal)
$ docker kill <container>

4) 𝗱𝗼𝗰𝗸𝗲𝗿 𝗱𝗶𝗳𝗳: An handy command to check any changes to:
-files
-directories 

on the container’s filesystem

A: added file or directory
C: changed file or directory was 
D: deleted file or directory

Usage:
docker diff <container_ID/container_name>

## VAGRANT
sudo vagrant up				>> ensure that .vagrant/machines/default/virtualbox/creator_uid is 0
sudo vagrant halt
sudo vagrant ssh
sudo yum -y install phpmyadmin
mysql -u root example -- just test
ifconfig (add IP ADRESS 192.168.50.52 + remote DENY )
sudo vim /etc/httpd/conf.d/phpMyAdmin.conf			>> KEYS: INSERT +  CTRL C + :w + :q
sudo service httpd restart

vim /etc/phpMyAdmin/config.inc.php
$cfg['Servers'][$i]['AllowNoPassword'] = TRUE;
+ MODIFY USER : root + secret

http://192.168.50.52/phpmyadmin 
root secret
exit

## LAMP

### Check

```
mysql -V
php -m
php -version
```

### Migrate

```
sudo apt install zip
sudo zip -r filename.zip foldername/
sudo unzip filename.zip -d directory
```

### Installation

- https://wiki.debian.org/LaMp
- https://www.tecmint.com/list-php-modules-in-linux/
- https://phoenixnap.com/kb/how-to-install-phpmyadmin-on-debian-10
- https://phoenixnap.com/kb/how-to-create-mariadb-user-grant-privileges
- https://stackoverflow.com/questions/869092/how-to-enable-mod-rewrite-for-apache-2-2
- https://www.howtoforge.com/tutorial/install-apache-with-php-and-mysql-lamp-on-debian-stretch/

```
sudo apt-get install php7.2-xml # add all the php package here
sudo apt install mariadb-server # install the mariaDB
sudo mysql_secure_installation # configure the mariaDB
sudo mysql # enter the mysql command line
sudo chmod 660 /var/www/html/phpmyadmin/config.inc.php
sudo chown -R www-data:www-data /var/www/html/phpmyadmin/
sudo service apache2 restart # check status of the apache server
sudo systemctl status apache2 # restart of the apache server
mysql -u pmauser -p dbname < dbfile.sql # execute sql file
sudo chown -R debian www # change file or folder owner (user:debian)
```

```
CREATE USER 'pmauser'@localhost IDENTIFIED BY 'mypwd';
GRANT ALL PRIVILEGES ON *.* TO 'pmauser'@localhost IDENTIFIED BY 'mypwd';
```

### Certificate

- https://www.snel.com/support/lets-encrypt-on-debian-9-with-apache-webserver/
- https://community.letsencrypt.org/t/the-requested-apache-plugin-does-not-appear-to-be-installed/95682/10

```
sudo apt-get install certbot
sudo apt-get install python-certbot-apache
sudo certbot --apache # new configuration
sudo certbot --apache -d example.com -d www.example.com # reconfigure
sudo certbot --apache -d hotelub.com -d www.hotelub.com # reconfigure
```

## NGINX

- https://github.com/agile6v/awesome-nginx

## CRON

crontab -e

Once you enter the above command you will be asked to choose a text editor. Choose nano if you are first time editing or go with your choice.

In the crontab, the m h dom mon dow user header has the following meaning

* m = The minute when the cron job will run. (0 to 59)
* h = A integer determining the hour when the tasks will run. (0 to 23)
* dom = Day of the Month when the cron job will run. (1 to 31).
* mon = The month when the cron job will run. (1 to 12)
* dow = Day of the Week from 0-6 with Sunday at 0. (0 to 6)
* user = The User under which the cron will run.
* command = The Linux command you wish to execute.


## DOMAIN CHECK

nslookup
set type=TXT
domain.fr


## PROCESS + UTIL

PUTTY

## SUPERVISION
htop

## MONITORING

- https://github.com/grafana/grafana

## UPDATE
aptitude update
aptitude upgrade

## UPDATE DATE
aptitude install ntp ntpdate
sudo nano /etc/ntp.conf

server 0.fr.pool.ntp.org
server 1.fr.pool.ntp.org
server 2.fr.pool.ntp.org
server 3.fr.pool.ntp.org
	   
service ntp start

## FIREWALLING 
iptable

vps1 et vps2  		> entree  22 pour tout le monde . et 80 si origin load balancer
sql					> entree  3389 depuis vps. et le 22 tout le monde

## CERTIFICATE

- https://certbot.eff.org/docs/using.html
