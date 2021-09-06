# code
https://inside-docupedia.bosch.com/confluence/display/BSC2OSD/Setup+U-Drive+Mount

\\KOR0FS07.APAC.BOSCH.COM\RPK2KOR$\

\\bosch.com\dfsrb\DfsDE\DIV\DS\engineering\projects\edc\medc17\97_Exchange\rpk2kor

sudo mount -t cifs -o user=RPK2KOR,cruid=RPK2KOR,sec=krb5 //KOR0FS07.APAC.BOSCH.COM/RPK2KOR$ ~/DriveU
sudo chown -R RPK2KOR. /home/rpk2kor/DriveU
# Example
sudo mount -t cifs -o user=$USER,cruid=$USER,sec=krb5 //bmh0fs01.apac.bosch.com/DOT5KOR$ /home/dot5kor/DriveU

\\si02fs13.de.bosch.com\medc17_2$\97_exchange

apt install cifs-utils keyutils
mount -t cifs  //si02fs13.de.bosch.com/medc17_2$/97_exchange /mount/bigdata_share -o username=RPK2KOR,workgroup=DE,uid=1218603084,vers=3.0

https://inside-docupedia.bosch.com/confluence/pages/viewpage.action?pageId=464987600
