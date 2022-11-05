# gpqhe
A C library doing fully homomorphic encryption under the license of LGPL.

## Package dependency

libgcrypt 1.10

# How to use

```sh
#step1: get gpqhe
git clonehttps://github.com/OChicken/gpqhe.git

#step2: install libgcrypt on Ubuntu
sudo apt-get install libgcrypt11-dev

#step3: build gpqhe
cd gpqhe
step3-1: 
#add "-std=c11" to CFLAGS in Makefile
#step3-2: 
make

#step4: build&run tests
cd tests
LD_LIBRARY_PATH=$PWD/../lib:$LD_LIBRARY_PATH
make test-gpqhe
./test-gpqhe enc sk
````

## Acknowledgement

HEAAN, NewHope, Kyber
