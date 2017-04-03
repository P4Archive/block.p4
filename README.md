# block.p4

Fuzhou University SDN Lab | P4

This repo is used to present the common function blocks in l2 switch that writed in P4.
We create the environment to test these blocks with mininet simulation tools.

## TODO

First copy the dirs `p4src` and `cmd` in the block such as port security to the `env` dir. 

Then do these:

```
cd env

./run_demo.sh
./add_entry.sh

cd mclearn
./mc_learn.sh
```

Then you can start these blocks with the env.

## SUPPORT FEATURES

0.features in `p4src`

1.port security

2.icmp security

3.udp flooding

4.port mirroring

5.resubmit

6.multicast NAT

7.trTCM

8.ECMP

9.TCP SYN/FIN check

## Demo

We have created two demo in dir `Demo`, `http_icmp_udp` and `sswitch`. 

The `http_icmp_udp` is a explaination example that one switch enabled the http security feature and another switch enabled both the icmp and udp security. See [http_icmp_udp](https://github.com/Emil-501/block.p4/tree/master/Demo/http_icmp_udp). 

The `sswitch` united all the blocks in one P4 switch pipeline, see [sswitch](https://github.com/Emil-501/block.p4/tree/master/Demo/sswitch) for more informations. 

The `DDoS` showed that how we defense the SYN/FIN/UDP DDoS attack with trTCM and TCP check. See [DDoS](https://github.com/Emil-501/block.p4/tree/master/Demo/DDoS).