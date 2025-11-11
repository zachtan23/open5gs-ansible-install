# open5gs-5GSA-ansible-install
Since installation may take time to read and understand, I create an easy way for people who want to setup fast and use. This ansible only auto install all the required of component, but it still need to manually change AMF's ngap address and upf address.
Please go sequence to run the auto installation. 

i) ansible-install.sh

ii) install.sh
After installation, please manually change the 2 IP address to fit your environment. 
a) vi /etc/open5gs/amf.yaml, and change the ngap address. 
b) vi /etc/open5gs/upf.yaml, and change the gtpu address.
c) Use webpage http://<IP_address>:9999, admin/1423 to login and create a subscriber account with IMSI, KI, OP/OPC. 

iii) verify.sh
