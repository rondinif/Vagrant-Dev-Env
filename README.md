# Vagrant-Dev-Env
Vagrant è di grande supporto nella realizzazione di macchine virtuali e del loro mantenimento. 
Grazie a Vagrant e Virtualbox è possibile costruire rapidamente l'ambiente di sviluppo di iGruppi.

# Requisiti
- [git](https://git-scm.com) - [Install git](https://git-scm.com/book/it/v1/Per-Iniziare-Installare-Git)
- [Virtualbox](https://www.virtualbox.org) - [Install Virtualbox](https://www.virtualbox.org/wiki/Downloads)
- [Vagrant](https://www.vagrantup.com) - [Install Vagrant](https://www.vagrantup.com/intro/getting-started/install.html)

# Installazione
Dopo aver installato Vagrant installare il [plugin Vagrant VBGuest](https://github.com/dotless-de/vagrant-vbguest):
```
$ vagrant plugin install vagrant-vbguest
```

Dopo aver installato i due software qui sopra creare una nuova directory di lavoro ed eseguire i seguenti comandi:
```
$ git clone https://github.com/iGruppi/iGruppi.git
$ cd iGruppi
$ git submodule update --init --recursive
$ cd ..
$ git clone https://github.com/iGruppi/Vagrant-Dev-Env.git
$ cd Vagrant-Dev-Env
$ vagrant up
```
A questo punto l'ambiente di sviluppo è raggiungibile all'indirizzo:
- iGruppi: http://localhost:8888/
- PhpMyAdmin: http://localhost:8888/phpmyadmin

Potrete modificare i sorgenti nella directory di lavoro e verificare direttamente il risultato sulla macchina virtuale appena creata e raggiungibile all'indirizzo qui sopra.
