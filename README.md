## Helping give NOMP new life! With some style.
#### If you want to help contribute, please look at the original [project](https://github.com/foxer666/node-open-mining-portal) first!

This is all the things great about NOMP, now with modern style and design of BootStrap 4! Having disliked the previous UI, due to cramping, little to no info displayed while what is displayed is not very helpful to users. I decided to fork a already great project, and add some stylistic touches it severely needs. I would of considered requesting pulls to the main branch, though with such heavy changes to the project, I decided a hard fork would be well suited. But if you would like to contribute, please consider looking at the [original project](https://github.com/foxer666/node-open-mining-portal) first, as these guys are the ones who helped get this NOMP rebirthing process started.

-------
### Node Open Mining Portal consists from 3 main modules:
* [NOMP](https://github.com/realcoin-rea/rea-nomp)
* [Stratum Pool](https://github.com/realcoin-rea/node-stratum-pool)
* [Node Multihashing](https://github.com/realcoin-rea/node-multi-hashing)

_Add new algorithms using [Node Multihashing](https://github.com/realcoin-rea/node-multi-hashing)._

Current version: v1.1.3

-------
### Recommended Dependencies/Setup Ubuntu 18.04
```
sudo apt-get install build-essential libtool autotools-dev autoconf pkg-config libssl-dev
sudo apt-get install libboost-all-dev libminiupnpc-dev redis-server
sudo apt-get install build-essential libsodium-dev npm libboost-all-dev
sudo apt-get install -y software-properties-common
sudo add-apt-repository ppa:bitcoin/bitcoin
sudo apt-get update
sudo apt-get install libdb4.8-dev libdb4.8++-dev
sudo apt-get -y install fail2ban
sudo systemctl enable fail2ban
sudo systemctl start fail2ban

sudo npm install -g n
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt-get install -y nodejs
```

-------
### Install
```
git clone https://github.com/realcoin-rea/rea-nomp.git
cd rea-nomp
npm install
npm start
```
-------
### Requirements
* Node 8.x.x or higher
* Coin daemon
* Redis Server

-------
### Hashing algorithms
#### Working
|   | Algorithm | Comment|
| ------------- | ------------- | ------------- |
| ✓ | __sha256csm__ | tested shares and payments with RealCoin (REA) |

#### Need tests
|   | Algorithm | Comment|
| ------------- | ------------- | ------------- |
| ? | __Argon2__ | need tests |
| ? | __Blake__ | need tests |
| ? | __Blake2S__ | need tests |
| ? | __Cryptonight__ | need tests |
| ? | __Dcrypt__ | need tests |
| ? | __Decred__ | need tests |
| ? | __Fresh__ | need tests |
| ? | __Fugue__ | need tests |
| ? | __GroestlMyriad__ | need tests |
| ? | __Quark__ | need tests |
| ? | __Hefty1__ | need tests |
| ? | __Keccak__ | need tests |
| ? | __Lbry__ | need tests |
| ? | __lyra2re__ | need tests |
| ? | __lyra2re2__ | need tests |
| x | __lyra2z330__ | need tests |
| ? | __NIST5__ | need tests |
| ? | __S3__ | need tests |
| ? | __Scrypt-N__ | need tests |
| ? | __Scrypt-OG__ | need tests |
| ? | __Sha1__ | need tests |
| ? | __SHAvite-3__ | need tests |
| ? | __Skein__ | need tests |
| ? | __X11Ghost__ | need tests |
| ? | __X13__ | need tests |
| ? | __X14__ | need tests |
| ? | __X15__ | need tests |
| ? | __zr5__ | need tests |
| ? | __ziftr__ | need tests |

-------

-------
### Credits
* [1301313Y](//github.com/1301313Y) - Upgraded the UI and stat modules
* [a2hill](//github.com/a2hill) - helped with X16r
* [devnulled](//github.com/devnull-ed) - helped with lyra2z, neoscrypt algo
* [Kris Klosterman / krisklosterman](https://github.com/krisklosterman) - Updated code for work wiht Node.JS >=8
* [Jerry Brady / mintyfresh68](https://github.com/bluecircle) - got coin-switching fully working and developed proxy-per-algo feature
* [Tony Dobbs](http://anthonydobbs.com) - designs for front-end and created the NOMP logo
* [LucasJones](//github.com/LucasJones) - got p2p block notify working and implemented additional hashing algos
* [vekexasia](//github.com/vekexasia) - co-developer & great tester
* [TheSeven](//github.com/TheSeven) - answering an absurd amount of my questions and being a very helpful gentleman
* [UdjinM6](//github.com/UdjinM6) - helped implement fee withdrawal in payment processing
* [Alex Petrov / sysmanalex](https://github.com/sysmanalex) - contributed the pure C block notify script
* [svirusxxx](//github.com/svirusxxx) - sponsored development of MPOS mode
* [icecube45](//github.com/icecube45) - helping out with the repo wiki
* [Fcases](//github.com/Fcases) - ordered me a pizza <3
* [yoshuki43](//github.com/yoshuki43) - his K-Nomp project has really help the development!
* Those that contributed to [node-stratum-pool](//github.com/zone117x/node-stratum-pool#credits)

-------
### License
Released under the GNU General Public License v2
http://www.gnu.org/licenses/gpl-2.0.html
