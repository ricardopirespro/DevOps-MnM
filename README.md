# DevOps-MnM

Tratamento de erros/avisos

hostnamectl set-hostname centos7.vbox

1.Para erros de acesso SSH rodar o comando:
config.ssh.insert_key = false
https://github.com/hashicorp/vagrant/issues/5059

set VAGRANT_PREFER_SYSTEM_BIN=0
https://stackoverflow.com/questions/51437693/permission-denied-with-vagrant

2.Para configurar o SMB host Windows com vm CentOS
https://github.com/hashicorp/vagrant/issues/11413

vagrant up
vagrant reload --provision
vagrant destroy -f

3. erro do vbguest

https://www.devopsroles.com/vagrant-no-virtualbox-guest-additions-installation-found-fixed/
vagrant plugin install vagrant-vbguest --plugin-version 0.21


ansible -m ping all


chmod 600 ~/.ssh/id_rsa
chown vagrant:vagrant ~/.ssh/id_rsa
