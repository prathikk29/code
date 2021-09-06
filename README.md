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



key
-----BEGIN PRIVATE KEY-----
MIIEvgIBADANBgkqhkiG9w0BAQEFAASCBKgwggSkAgEAAoIBAQCeQ9tGtauX7R3c
GeYJtPTHF4xcaDtToxOirGpHMQjWl//IZ9qDT/glI7nzVu/POrivRqDEJPGp47uL
iCG0bZ+4WlI7vZGjCNBFTYxFlu8RWL/xEEfaaHz2SYcLrQYXss0omxgVsIj82D/B
TME5WRlOdcGN0a6FOH/a22CTfZ2LefGcfWnBY/++yLYE4v8pE+DCETEIm6DPXb2T
+gArZSdtj5TC2Hh6AxpPs76w1rJVn5/e9bF9pZQMuB2kTblbACg3PYSutl0CsqIc
24xbWpPqxWzNffbOpAznJuQnMY0okcoAYkuYnouN8eMkRKYrQ/aIIGQNSkmA5bpr
NtefwsShAgMBAAECggEAHmOZLzKjCEEXgrPWX/bHKZNz+CpredvOYWYJ4jGgKNR2
4NxQMPaiBz+c7QS8d2YnIEDHjeIqJRz9XgV9s095Y8S0FZSI6m0+0I/bZ2Fb9lC8
SmV95oo5tHDZ5XwLt3E1w55EOaX0J9i+JTe/wmtBWLdzuu+QOzRmGHgXSzrLjYRH
eTxqLRJglfDBU6xNJgeScOhZOYxQ5MGpo+T1FAU4YdXi4T+JN2lcOIQ18QDJZYCX
VxfWoF+mcxZpbv9k7STJFxciYXA8qmiFXyOaQp+qNRggCgcQes6uR5RQn6Yelds6
GeOLokXhubR4jqAHnIDPlyIj0vIBKvKjoripuf7PgQKBgQDMYiA8OSDTSfpH9HKk
wBY6Ihoj5mDH9TvsBC8y4Vm8kiwXVS7kas0+xwPUzwdRDc/Xm+DU45YI4Mxqf/1F
Dz7TTXrHU2mYN2QBTFv3zMM5D4q5Pb1Ffnlw6bK9iwLA+4AMwl4azfQtlwKmNrOn
TEb3sZfeg0e8a5yIesdr/rntlQKBgQDGPBM4u0WpmgxJ2C1I8udYVYiAzsqAnyp6
DclRQbKhjxiH3Js038x8nVjgLIlZqo7pJKolggJil49Uo5CoxUq5vKzm2GYIcV2a
9mYAKx0yZgElxAM0ctk2zBa69EEPookIfV9hAks96XaY0RLnLjy1cMgYZUYB1ZMc
WP5iTGU/3QKBgQCk8hBn6gcW3l5SEfMwCSInGnyUOooi9kS87oeU/Y+pgyJ4VjP4
/kTUhFMQPWD/RjFWJaQmy+G7Gol+7fpd8LbYW3BaS3Qt944LCjAy5ZssguGHLE+D
NVYXDVRGalj3nEG0imzeHxcQcA4gTIdi3klr/3S8jKCpbQOwlb455yLwnQKBgCob
nrWhSgXhvBR/f/cL6cpguNMrmeZCaQJuJUJGY0xgGgTZ/nn3w/cAcV2E+FP8n8i0
ShQXjqwkp4SCDftblSjpBA0xEFNgyVJeXoJQpi4Lbtj3zvp4Ht298mIZ+iv5CYSt
JPJ1S0hGbDO/zXUf5DNiVo6gDIPdOxd9a+OzeJpdAoGBALAHcqBAwksYc/dwzCe4
71m0f87Rj5mm7nUC3q6aeRZbgWF/7KLCc1fNYr4fr5OrH0pelN11v5h1TQWod3l0
t7jVvGXIf5VpTybo1IUIEGHYj6Li763BuHzv83U3G/8/a/8g2RSIT8d8fe96Ji5z
oZQMJ94Y0CHxoFgxVlOIRZD6
-----END PRIVATE KEY-----

cert

