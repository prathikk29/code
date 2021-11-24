# code
https://inside-docupedia.bosch.com/confluence/display/BSC2OSD/Setup+U-Drive+Mount

$connectTestResult = Test-NetConnection -ComputerName "https://testfleabox.blob.core.windows.net/testforvm" -Port 445
if ($connectTestResult.TcpTestSucceeded) {
# Save the password so the drive will persist on reboot
cmd.exe /C "cmdkey /add:`"https://testfleabox.blob.core.windows.net/testforvm`" /user:`"testfleabox`" /pass:`"bpzmeSUrKR6Kp61JdvYntSmdg6lEsKbth5CSy2SRoAhXWMHDW03tS4k0etvqr7mabGPOCLC49lkVDoenZE6H2Q==`""
# Mount the drive
New-PSDrive -Name Z -PSProvider FileSystem -Root "\\https://testfleabox.blob.core.windows.net/testforvm/testvm.txt\" -Persist
} else {
Write-Error -Message "Unable to reach the Azure storage account via port 445. Check to make sure your organization or ISP is not blocking port 445, or use Azure P2S VPN, Azure S2S VPN, or Express Route to tunnel SMB traffic over a different port."
}
(New-Object -ComObject Shell.Application).NameSpace('Z:').Self.Name = 'Azure Blob Storage'

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
-----BEGIN CERTIFICATE-----
MIIGWzCCBUOgAwIBAgIEXSHmszANBgkqhkiG9w0BAQsFADBRMRMwEQYKCZImiZPy
LGQBGRYDY29tMRUwEwYKCZImiZPyLGQBGRYFQm9zY2gxDDAKBgNVBAMTA1BLSTEV
MBMGA1UEAxMMQm9zY2gtQ0ExLURFMB4XDTIxMDkwMzA5NDYzMVoXDTIzMDkwMzEw
MTYzMVowbjETMBEGCgmSJomT8ixkARkWA2NvbTEVMBMGCgmSJomT8ixkARkWBUJv
c2NoMQwwCgYDVQQDEwNQS0kxEDAOBgNVBAMTB01hY2hpbmUxIDAeBgNVBAMTF3Np
MHZtYzQwMTIuZGUuYm9zY2guY29tMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
CgKCAQEAnkPbRrWrl+0d3BnmCbT0xxeMXGg7U6MToqxqRzEI1pf/yGfag0/4JSO5
81bvzzq4r0agxCTxqeO7i4ghtG2fuFpSO72RowjQRU2MRZbvEVi/8RBH2mh89kmH
C60GF7LNKJsYFbCI/Ng/wUzBOVkZTnXBjdGuhTh/2ttgk32di3nxnH1pwWP/vsi2
BOL/KRPgwhExCJugz129k/oAK2UnbY+Uwth4egMaT7O+sNayVZ+f3vWxfaWUDLgd
pE25WwAoNz2ErrZdArKiHNuMW1qT6sVszX32zqQM5ybkJzGNKJHKAGJLmJ6LjfHj
JESmK0P2iCBkDUpJgOW6azbXn8LEoQIDAQABo4IDHDCCAxgwCwYDVR0PBAQDAgWg
MB0GA1UdJQQWMBQGCCsGAQUFBwMBBggrBgEFBQcDAjCCAUYGA1UdIASCAT0wggE5
MIIBNQYNKwYBBAGpRoN9AQICATCCASIwLAYIKwYBBQUHAgEWIGh0dHA6Ly90cnVz
dGNlbnRlci5ib3NjaC5jb20vY3BzMIHxBggrBgEFBQcCAjCB5BqB4VRoZSBCb3Nj
aCBDZXJ0aWZpY2F0aW9uIFByYWN0aWNlIFN0YXRlbWVudCAoQ1BTKSBhdmFpbGFi
bGUgYXQgaHR0cDovL3RydXN0Y2VudGVyLmJvc2NoLmNvbS9jcHMgaXMgaGVyZWJ5
IGluY29ycG9yYXRlZCBpbnRvIHlvdXIgdXNlIG9yIHJlbGlhbmNlIG9uIHRoaXMg
Q2VydGlmaWNhdGUuIFRoaXMgQ1BTIGNvbnRhaW5zIGxpbWl0YXRpb25zIG9uIHdh
cnJhbnRpZXMgYW5kIGxpYWJpbGl0aWVzLjAiBgNVHREEGzAZghdzaTB2bWM0MDEy
LmRlLmJvc2NoLmNvbTCCAS8GA1UdHwSCASYwggEiMGugaaBnpGUwYzETMBEGCgmS
JomT8ixkARkWA2NvbTEVMBMGCgmSJomT8ixkARkWBUJvc2NoMQwwCgYDVQQDEwNQ
S0kxFTATBgNVBAMTDEJvc2NoLUNBMS1ERTEQMA4GA1UEAxMHQ1JMMzYyMzCBsqCB
r6CBrIZmbGRhcDovL2Jvc2NoLmNvbS9jbj1XaW5Db21iaW5lZDIsY249Qm9zY2gt
Q0ExLURFLGNuPVBLSSxkYz1Cb3NjaCxkYz1jb20/Y2VydGlmaWNhdGVSZXZvY2F0
aW9uTGlzdD9iYXNlhkJodHRwOi8vdHJ1c3RjZW50ZXIuYm9zY2guY29tL0NSTC9i
b3NjaC1jYTEtZGVfcGtpX2NvbV9jcmxmaWxlMi5jcmwwHwYDVR0jBBgwFoAU3gTi
zIkI/XWM2KQwMdgQbeWh9JswHQYDVR0OBBYEFL9bRlVR7tau0UWb6sShOk2FxRRW
MAkGA1UdEwQCMAAwDQYJKoZIhvcNAQELBQADggEBAFFZ/AzxflLpmIP0Xe+Zng5Q
rXjlwS7cEoWe9tsi4GzM1SKi3BsJb0fSiEgepNgNlWvZc2W8Cse62pAM+X5Rt/Ta
UUDbxX/8zZ4FtofYhzs+K9vvPryQUpl6RgmZuocXHudoM6zwSXMCDvkR+cBxj19D
+Mah8IcuRTg27eqclb3zk5ks8jD8EuvSRDyY7y7O7icBmWQ0pqbRkT//B0n3sQWq
0b2LHijhvQfEfxaJqS1NbWbkXMw+v7sKzNWGz32XeTFLS1/K3KV5s4x/MCF3QyZO
/pEXlj8jnLzI1fv9ty5TClPa9dYfq0XnVWLA7trDP4V538yPjCui4d/lhSdwkwU=
-----END CERTIFICATE-----

$connectTestResult = Test-NetConnection -ComputerName "https://testfleabox.blob.core.windows.net/testforvm" -Port 445
if ($connectTestResult.TcpTestSucceeded) {
    # Save the password so the drive will persist on reboot
    cmd.exe /C "cmdkey /add:`"https://testfleabox.blob.core.windows.net/testforvm`" /user:`"testfleabox" /pass:`"bpzmeSUrKR6Kp61JdvYntSmdg6lEsKbth5CSy2SRoAhXWMHDW03tS4k0etvqr7mabGPOCLC49lkVDoenZE6H2Q=="
    # Mount the drive
    New-PSDrive -Name Z -PSProvider FileSystem -Root "\\https://testfleabox.blob.core.windows.net/testforvm" -Persist
} else {
    Write-Error -Message "Unable to reach the Azure storage account via port 445. Check to make sure your organization or ISP is not blocking port 445, or use Azure P2S VPN, Azure S2S VPN, or Express Route to tunnel SMB traffic over a different port."
} 
(New-Object -ComObject Shell.Application).NameSpace('Z:').Self.Name = 'Azure Blob Storage'

