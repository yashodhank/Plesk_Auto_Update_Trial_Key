[![Build Status](https://travis-ci.com/megoRU/Plesk_Auto_Update_Trial_Key.svg?branch=master)](https://travis-ci.com/megoRU/Plesk_Auto_Update_Trial_Key) 
![GitHub All Releases](https://img.shields.io/github/downloads/megoRU/Plesk_Auto_Update_Trial_Key/total) 
[![GitHub stars](https://img.shields.io/github/stars/megoRU/Plesk_Auto_Update_Trial_Key)](https://github.com/megoRU/Plesk_Auto_Update_Trial_Key/stargazers)
[![GitHub license](https://img.shields.io/github/license/megoRU/Plesk_Auto_Update_Trial_Key)](https://github.com/megoRU/Plesk_Auto_Update_Trial_Key/blob/master/LICENSE)

## Disclaimer
<b>I am against the abuse of free licenses. This code is presented for informational purposes only. Using it can and probably violates Plesk rules. The author is not responsible for any material losses incurred by Plesk.</b>

# Plesk auto-update trial key
Plesk trial key auto update

## Create table in MySQL:

```
CREATE TABLE `Plesk` (
  `id` int(6) NOT NULL,
  `text` varchar(255) NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `text` (`text`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;
```
```
INSERT INTO Plesk (id, text) values (0, "Your Key");
INSERT INTO Plesk (id, text) values (1, "Your Key2");
INSERT INTO Plesk (id, text) values (2, "Your Key3");
```

##  Run on Windows:
bat file<br>
java -jar Plesk_Auto_Update_Trial_Key.jar "ip address MySQL" "user MySQL" "pass MySQL" "ip address SSH" "login SSH" "pass SSH" "database name mysql"

## Run on Linux (Debian/Ubuntu):
sudo apt-get install screen <br>
sudo apt-get install openjdk-15-jdk <br>
export JAVA_HOME=/usr/lib/jvm/openjdk-11-jdk <br>
export PATH=$PATH:$JAVA_HOME/bin <br>
java -version <br>

screen -dmS pleskKey bash -c "java -jar Plesk_Auto_Update_Trial_Key.jar "ip address MySQL" "user MySQL" "pass MySQL" "ip address SSH" "login SSH" "pass SSH" "database name mysql" "

## Get free key:
https://www.plesk.com/plesk-free-download/ <br>
https://temp-mail.org/ru/ <br>

## Ideological inspirer

[yashodhank](https://github.com/yashodhank)

## FAQ & Troubleshooting

• On Windows/MacOS, install Oracle Java from [here](https://www.oracle.com/java/technologies/javase-downloads.html) or OpenJDK from [here](https://adoptopenjdk.net/).
