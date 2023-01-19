super user : postgres
mot de passe : adm1adm1
alter role segma with password 'segma';
alter database segma owner to segma;
alter role segma login;


CREATE TABLE utilisateurs (
   username varchar(15) NOT NULL,
   password varchar(150) NOT NULL,
   role varchar(15) NOT NULL,
   Primary key (username)
   );
INSERT INTO utilisateurs (username, password, role)
 VALUES
 ('admin', 'admin', 'administration'),
 ('user', 'user', 'etudiant');
 
 sudo dnf install -y httpd
 sudo systemctl start httpd

sudo systemctl status httpd
sudo systemctl enable httpd
 sudo dnf install php
 sudo dnf install php-pgsql
sudo yum install php-json

sudo yum install jq -y
sudo setsebool httpd_can_network_connect 1
sudo setsebool httpd_can_network_connect_db 1
sudo yum install git
