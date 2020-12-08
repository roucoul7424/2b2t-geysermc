# 2b2t-geysermc
<img src="https://1.bp.blogspot.com/-a5R7P_h1ivs/X8_EMFyoH4I/AAAAAAAAAlg/yqiLYQLcZCcfFKgaWU934hbLtrqGw-xqwCLcBGAsYHQ/w945-h600-p-k-no-nu/untitled.png"/>

application needed:

-Termux

-Geysermc app : https://ci.rtm516.co.uk/job/GeyserAndroid/job/master/

-minecraft pockect edition

you also need a java account of minecraft (pc account)
-----------------------------------------------------------------------------

Francais : 

application necessaire : 

Termux

geysermc : https://ci.rtm516.co.uk/job/GeyserAndroid/job/master/

minecraft pocket edition

vous avez aussi besoin d'un compte java de minecraft (pc)
-----------------------------------------------------------------------------



# command:
<img src="https://cdn-images-1.medium.com/max/947/1*IdpTMzcLP9HrI7GVYKfLgA.png" alt="HACKING ANDROID WITH TERMUX | LaptrinhX"/>

open termux and type down the following commands :
-

`curl https://gist.githubusercontent.com/rtm516/e3e07d6595ee41e05a38b03c0f4d7a80/raw/install.sh | bash`

`cd ~/ubuntu_directory/start-ubuntu.sh`

`mkdir bungee`

`cd bungee`

`apt install wget`

`wget https://ci.md-5.net/job/BungeeCord/lastSuccessfulBuild/artifact/bootstrap/target/BungeeCord.jar
java -jar BungeeCord.jar`

`end`

`cd plugins`

`wget https://ci.viaversion.com/job/ViaVersion/lastSuccessfulBuild/artifact/jar/target/ViaVersion-3.2.1-SNAPSHOT.jar`

`cd ..`

`java -jar BungeeCord.jar`

`end`

`sed -i 's/default: 47/default: 340/g' plugins/ViaVersion/config.yml`

`apt install screen`

`cd ~`

`mkdir proxy`

`screen -S proxy bash`

`cd proxy`

`curl -sL https://deb.nodesource.com/setup_15.x | bash -`

`apt-get install -y nodejs`

`git clone https://github.com/PrismarineJS/node-minecraft-protocol`

`cd node-minecraft-protocol`

`cd examples/proxy`

`nano proxy.js`

Go to where it says:

  `const targetClient = mc.createClient({
    host: host,
    port: port,
    username: client.username,
    keepAlive: false,
    version: version
  })`

(on line 94)

Change it to:

  `const targetClient = mc.createClient({
    host: host,
    port: port,
    username: 'your.java.edition.login@email.com',
    password: 'your_minecraft_password'
    keepAlive: false,
    version: version
  })`
  
Ctrl + O, enter, Ctrl + X
