### Document
* [Install Tutorial](http://thrift.apache.org/docs/install/)
* [Build from source](http://thrift.apache.org/docs/BuildingFromSource)

### Install thrift in ubuntu
```bash
sudo apt-get install automake bison flex g++ git libboost-all-dev libevent-dev libssl-dev libtool make pkg-config
wget https://mirror.bit.edu.cn/apache/thrift/0.13.0/thrift-0.13.0.tar.gz
tar -xzvf thrift-0.13.0.tar.gz
cd thrift-0.13.0
./bootstrap.sh
./configure
make
make check
sudo make install
```


