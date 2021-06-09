# Integrantes

* Alexandre
* Camila
* Gercino
* Luan
* Nikolas

# Version Information

* Hadoop 2.7.3
* Spark 2.1.1
* Zeppelin 0.8.0 

# Web user interfaces

* HDFS: (http://node1:50070/dfshealth.html)
* Spark history server: (http://node1:18080)
* Zeppelin: (http://node1:8080)

# Vagrant VM

```
vagrant up --provider="virtualbox"

vagrant ssh node1

cd /vagrant/
```


# Create Directories in HDFS

```
hdfs dfs –mkdir –p ocorrencias

hdfs dfs –put si_env-2019.csv /user/vagrant/ocorrencias
hdfs dfs –put si-bol-2019.csv /user/vagrant/ocorrencias
hdfs dfs –put si-log-2019.csv /user/vagrant/ocorrencias

```

# Start Zeppelin

```
sudo /home/ubuntu/zeppelin/bin/zeppelin-daemon.sh start
```
