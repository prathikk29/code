# code
https://inside-docupedia.bosch.com/confluence/display/BSC2OSD/Setup+U-Drive+Mount

\\KOR0FS07.APAC.BOSCH.COM\RPK2KOR$\

\\bosch.com\dfsrb\DfsDE\DIV\DS\engineering\projects\edc\medc17\97_Exchange\rpk2kor

\\si02fs13.de.bosch.com\medc17_2$\97_exchange

sudo apt install cifs-utils keyutils
sudo mount -t cifs  //si02fs13.de.bosch.com/medc17_2$/97_exchange /mount/bigdata_share -o username=RPK2KOR,workgroup=DE,uid=$UID,vers=3.0

https://inside-docupedia.bosch.com/confluence/pages/viewpage.action?pageId=464987600
