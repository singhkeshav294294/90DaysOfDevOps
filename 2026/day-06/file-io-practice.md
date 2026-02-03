Last login: Mon Feb  2 10:17:40 on ttys000
keshavsingh@dhcp-10-48-12-102 ~ % touch notes.txt
keshavsingh@dhcp-10-48-12-102 ~ % echo "hello" > notes.txt 
keshavsingh@dhcp-10-48-12-102 ~ % echo "hello2" >> notes.txt
keshavsingh@dhcp-10-48-12-102 ~ % cat notes.txt 
hello
hello2
keshavsingh@dhcp-10-48-12-102 ~ % echo "hello3" > notes.txt 
keshavsingh@dhcp-10-48-12-102 ~ % cat notes.txt 
hello3
keshavsingh@dhcp-10-48-12-102 ~ % echo "hello2" >> notes.txt
keshavsingh@dhcp-10-48-12-102 ~ % echo "hello3" >> notes.txt
keshavsingh@dhcp-10-48-12-102 ~ % echo "hello5" >> notes.txt
keshavsingh@dhcp-10-48-12-102 ~ % echo "hello6" >> notes.txt
keshavsingh@dhcp-10-48-12-102 ~ % cat notes.txt 
hello3
hello2
hello3
hello5
hello6
keshavsingh@dhcp-10-48-12-102 ~ % cat notes.txt | head
hello3
hello2
hello3
hello5
hello6
keshavsingh@dhcp-10-48-12-102 ~ % cat notes.txt | head 2
head: 2: No such file or directory
keshavsingh@dhcp-10-48-12-102 ~ % cat notes.txt | tail  
hello3
hello2
hello3
hello5
hello6
keshavsingh@dhcp-10-48-12-102 ~ % echo "hello" | tee notes.txt
hello
keshavsingh@dhcp-10-48-12-102 ~ % cat notes.txt 
hello mc
keshavsingh@dhcp-10-48-12-102 ~ % cat << heloo | tee notes.txt 
hello
keshavsingh@dhcp-10-48-12-102 ~ % 
keshavsingh@dhcp-10-48-12-102 ~ % cat << heloo bsc | tee -a notes.txt
hello bsc
keshavsingh@dhcp-10-48-12-102 ~ % cat notes.txt 
hello bsc
keshavsingh@dhcp-10-48-12-102 ~ % 
