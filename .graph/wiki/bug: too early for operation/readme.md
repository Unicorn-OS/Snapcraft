# Problem:
error: too early for operation, device not yet seeded or device model not acknowledged

sch: https://www.google.com/search?q=error%3A+too+early+for+operation%2C+device+not+yet+seeded+or+device+model+not+acknowledged
https://www.google.com/search?q=too+early+for+operation%2C+device+not+yet+seeded+or+device+model+not+acknowledged

bug-report:
https://bugs.launchpad.net/snapd/+bug/1826662

# Solution:
https://www.unixcloudfusion.in/2022/07/solved-too-early-for-operation-device.html

https://bugs.launchpad.net/snapd/+bug/1826662/comments/7

1.  
"One suggestion is to run this before attempting any snap install, et al commands:

snap wait system seed.loaded"


2.  
"Simply doing a:

systemctl restart snapd.seeded.service

Was sufficient to get everything working for me."