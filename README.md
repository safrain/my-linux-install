# my-linux-install

sudo apt-get install vim

wget "http://download.oracle.com/otn-pub/java/jdk/8u45-b14/jdk-8u45-linux-x64.tar.gz"
tar -zxf jdk-8u45-linux-x64.tar.gz
sudo mv jdk1.8.0_45/ /usr/lib/jdk
sudo update-alternatives --install /usr/bin/java java /usr/lib/jdk/jre/bin/java 30
sudo update-alternatives --install /usr/bin/javac javac /usr/lib/jdk/bin/javac 30


export JAVA_HOME=/usr/lib/jdk/
export JRE_HOME=/usr/lib/jdk/jre
export CLASSPATH=.:${JAVA_HOME}/lib:${JRE_HOME}/lib
export PATH=${JAVA_HOME}/bin:$PATH
export ANDROID_HOME=~/opt/android-sdk-linux

mkdir bin

sudo vim /etc/rc.local
 -> sudo mount -t vboxsf shared /shared
