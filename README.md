# Installing cpuminer-multi on your Pi
Here you can find the commands used in the BloxyLabs videos about cpu-miner multi and mining for example Bitcoin.
<br>
<br>
Check also our YouTube channel for instructions and other related information [YouTube](https://www.youtube.com/@bloxylabs "YouTube").
<br>
If you had fun with the projects, please consider giving us a Super Thanks on YouTube or buying us a [cup of coffee](https://www.buymeacoffee.com/bloxylabs "cupofcoffee").


**Command to update the OS:**

```
sudo apt update
```

**Command to upgrade the OS:**

```
sudo apt upgrade -y
```

**Command to install screen:**

```
sudo apt install screen
```

**Command to install libraries and other dependecies:**

```
sudo apt-get install git automake libcurl4-openssl-dev pkg-config libjansson-dev libssl-dev libgmp-dev zlib1g-dev make g++ autoconf
```

**Command to get the required code:**

```
git clone https://github.com/tpruvot/cpuminer-multi
```

**Command to auto generate:**

```
sudo ./autogen.sh
```

**Command to configure cpuminer-multi:**

```
sudo ./configure --disable-assembly CFLAGS="-Ofast -march=native" --with-crypto --with-curl
```

**Command to build/compile cpuminer:**

```
sudo ./build.sh
```

**Command to start mining Bitcoin using sha256d:**

```
./cpuminer -a sha256d -o stratum+tcp://POOLADDRESS:PORTNUMBER -u WALLETADDRESS.WORKERNAME -p PASSWORD
```

**Command to check cpu temperature:**

```
vcgencmd measure_temp
```

Interested in mining Bitcoin at home with small miners or just looking for cool Bitcoin merchandise? Check out BitcoinMerch.com. You will get a 5% discount by using the code BloxyLabs. Visit their website by clicking the banner below to support the channel
[![Alt text](bitcoinmergebanner.jpg)](https://bitcoinmerch.com?aff=706)
