# FlareOS
simple os

## How to run
1. Clone the repository
2. run ```docker build -t flareos-buildenv buildenv```
3. run ```docker run -it --rm -v $(pwd)/..:/root/env -v $(pwd)/storage:/root/storage flareos-buildenv```
4. run ```cd /root/env```
5. run ```make build-x86_64```
6. exit container then run ```qemu-system-x86_64 -cdrom dist/x86_64/kernel.iso```