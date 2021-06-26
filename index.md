## Firework BLOCK CHAIN
### Peakadness structure of hierarchy block chain

The theory mainly elaborate what is Firework block 
chain, and it’s key implementation, including 
consensus, hierarchy, network and high performance 
algorithm, meanwhile, also telling Firework block 
chain usage sense, how to use it to constitute a 
digital currency biosphere, development advice and 
running environments.

## Author

<p>
  <span>Jazping</span>
</p>

## Directory
```
Key words................................................................................2
Explanation..............................................................................2
Summary description .....................................................................3
Block chain..............................................................................3
Digital currency description.............................................................3
Purpose of born..........................................................................4
Consensus mechanism .....................................................................5
Stratified mechanism ....................................................................6
Structure philosophy ....................................................................8
Nerve of network.........................................................................8
Cache policy ............................................................................10
Synchronized policy......................................................................10
Transaction contract.....................................................................12
High available...........................................................................13
Cipher and safety .......................................................................13
Store system ............................................................................14
Immortalized solution ...................................................................15
Development .............................................................................16
Running environment .....................................................................17
Bibliography ............................................................................19
```

## Key words

Block chain Philosophy, Block chain hierarchy, NPOS, Forest block chain, Firework 
block chain

## Explanation

<p><b>Hbase</b> is one distributed big data store database and the top project of Apache</p>
<p><b>NIO</b> is one that non-blocking asynchronous correspondence specification</p>
<p><b>Netty</b> is one NIO operation framework that contains many encoding</p>
<p><b>PhotonIO</b> is based on netty or mina and microminiaturization of protocoled 
operation framework</p>
<p><b>Galaxy</b> is one abstract consensus region cluster</p>
<p><b>NPOS</b> is one decentralized consensus mechanism</p>
<p><b>Nebula Hash</b> is one that multiple concurrent consensus hash</p>
<p><b>Ocean Contract</b> represent open</p>
<p><b>DOCWTO</b> indicate digital ocean contract world trade organization</p>

## Summary description

### Block chain
<p>What the hell is block chain? For this question, author ponders for a long time 
before write this, but has no absolutely answer about that, after taking the actual 
action and make unremitting probe, and find the follow conclusion by it shelf
finally.</p>
<p>In the true, block chain is one serious data that generate by different district, 
and organized to be a chain, the chain has traceability of data from, and anyone 
can recognize that, but cannot change it.</p>
<p>Block chain is a database that running in distributed account book with 
consensus mechanism. The meaning of this technique is shading the retrospect 
able transaction data for anyone, so that achieve the decentralization. Besides, 
technique traits of block chain using the machine to machine supplant the human 
to human mechanism and dislodge the suspicion in human.</p>

### Digital currency

<p>Digital currency definition so wide, the understanding of digital currency of 
pseudonym is that, must has cipher effect, safely transport in consensus 
mechanism, initiated by finance purpose and serve the finance business, the estate 
in Firework account book not allowed manual modify to increase the amount, but 
how much estate one address has, anyone can seem clearly. But, the address 
cannot fetch the people name, so you only can know the property of address; never 
know the property of people.</p>
<p>Original Firework block chain not proffer ability of currency mine, but we can 
implements privately, we can predestine one batch of address that contains balance 
and missing token, one must figure out the match token by a lot of computing try, 
so that the token satisfied predestine account verification, if so, one can transmit 
the balance of this address to their own address. Besides, we also can make many 
conduct transaction, but the data not completed, miner must figure out the missing 
data make it through the verification, so that can impel the miner to mining.</p>

## Natal Purpose

<p>In generally speaking, it has no difference from generic block chain; all are 
working by common account book in consensus mechanism and decentralized 
‘database’. But in implementation there are many differences from other block 
chain. It deem that developer change the configuration and digital product name 
for new digital currency. Generic block chain store data in local file not support 
distributed data verification and big data analysis. But the forest block chain 
reckons store transaction data in distributed system like Hbase as layer of storage, 
so that to support big data analysis for transaction, such as a phase of transaction 
amount and district. And the advantage in data verification celerity when data 
come out to large, because of the real distributed region is computing concurrently. 
It main purpose is to build a biosphere of block chain like digital finance, overbear 
large amount transaction.</p>

## Consensus mechanism

<p>There some prevalent consensus algorithm in block chain at present, they are 
respectively POW, POS, DPOS and PBFT, But forest block chain using NPOS that 
created by author. It’s mechanism is select the near peer servers to consensus the 
computing, we called that peer servers as one galaxy, the amount of this peer 
servers general 9, but we can change it by configuration if we want. This away has a 
weakness is, only few servers participate in consensus and easy to attack. Although
the cracker maybe penetrate one galaxy, but if try to modify any transaction record, 
that will be make the penetrated server to be insular, and cannot take part in other 
consensus anymore, and trigger the server run synchronized programme. So that 
the cracker want penetrated one galaxy, they need to penetrate them at same time. 
If the cracker did these, the follow thing they need is expand byzantine attack, the 
amount of server the crack has, determined they whether success. However, the 
algorithm advantage is low cost and high performance, after the galaxy consensus, 
the servers push this message to superior or subordinate or the peer that is not 
participated in this consensus. If you know the COVID-19 spread way, then you 
know the way of this consensus. No matter how to push the consensuses, other 
server if don’t know the transaction, they need to check and consensus again to 
confirm the data is legal. If manual make one illegal message send to them, they 
just skip the message and do nothing. This consensus method deepens the 
decentralization.</p>
<p>We recommend list the consensus server to one website or gateway server, 
then configure consensus path refer to this URL, so that all server can check the 
consensus sources every day, and make new cluster to replace the yesterday, so 
that no one know one server connected to where, and animate the consensus 
source. Forest block chain do these at one day as period, the minimum interval is 
two hours. Besides, if we centralized the consensus sources that will be equivalent 
control the ‘nuclear fusion’. If one region of server is out of control, we can 
dislodge them out. But there good and bad things when do like this, in the relative
world, nothing is perfectly. If cracker penetrated the consensus source and pull it 
refer to one that they want, the absolutely puissance will be control by them.</p>

## Stratified mechanism

<p>Another trait of Firework block chain is support stratified design, in unlimited
user amount sense, we can stratify by district to dissipate user transaction request. 
But all stratification has no limitation in server node, the more server node the 
safety. It is require that just allow one node account for upper stratification in same 
district region, or will occur one upload transaction data while another throw 
duplicate hash, that is waste of resources. This account book of the region will be 
unanimous finally, but there is difference output about user transaction. If one user 
do transaction at one place tomorrow does transaction at another place is no 
problem. But if do transaction at multiple place at same time, that ought to avoid. 
First of all, data synchronize is not fast enough; second, one address do transaction 
at same time cannot consensus. If you know the space-time overlap in science 
fiction, that you know why so is that. Because of one of you only allow present at 
one space-time at same time, if multiple you present will cause the serious problem. 
To avoid this situation, we need to exalt the count of consensus server or by request 
gateway to conduct user transaction. But also cannot avoid the byzantine problem.</p>
<p>All layer of server count at least 9, the development count configure to 3, 
consensus count configure to 9, although server count more exceed 9, but 9 
consensus server already enough for do transaction. If one transaction success 
consensuses, that will be trigger chain reaction and diffuse it to all server at finally. 
This situation can save the delay of distance between servers. However, the servers 
in the galaxy no need to set by manual, let those select automatically.</p>
<p>The galaxy servers will trigger chain reaction after they consensus one 
transaction, system also push the data to upper chain too, so that all server know 
the transaction record. The typical scene is the strut like country, province, and city, 
county. It is high delay in hierarchy, the reason is for deplete upper chain pressure 
of data processing. So the upper layer server only invoke by lower layer server, not 
invoke by user directly.</p>

## Structure philosophy

<p>So called Firework block chain is because one trait that it is not single chain, 
there will be many chain genesis with an root block, so that to promote the 
transaction ability. The previous block of every transaction record select by random 
way, so that will generate many chain like a tree, algorithm try to keep that one 
block only has one child, but the amount of node that initiate phase too few to 
keep them one child only, for this reason it have to reuse the duplicated parent 
node. But by time going, chains will become more and more, leaf more and more 
too, the high of tree will be higher and higher, and then one block only has one 
child will come true. That will cause more and more region present after enough 
server join in the cluster. You can imagine the course of one firework explode in 
darkness sky to disappear, to help you understand why called Firework block chain. 
If you understand the evolution of university, that will easy to grasp this philosophy.</p>

## Nerve of network

<p>Another trait of Firework block chain is that, its network base on NIO, take the 
most popular framework called Netty as NIO underlying, it is fast, nimble in 
configuration, we can adopt select mode in windows operation system and also can 
adopt epoll in Linux operation system. Besides, we can configure system boot 
argument like memory distribution and direct type of heap type. However, firework 
block chain network nerve is not build in Netty directly, there is one middleware 
which support protocoled NIO, it is another composition of author called PhotonIO, 
this component mainly resolve data packet tackiness and overlap, provide an 
sample program environment. The PhotonIO not proper to process big packet, 
strive to keep small packet transmit, this network not allow blocking code existence, 
so that is demanding to coding.</p>
<p>Firework block chain network valid the connective server automatically, it will 
dislodge server that if the server in the cluster was disconnected. If there is 
insufficient consensus server in cluster, it will try to find substitute from consensus 
source, so that insure amount of consensus server. But the disconnected server will 
join again if the server reconnected. System try to keep the consensus amount 
which configure by manual, if one server has enough connection to outside, it also 
can receive new connection from outside, but not establish new connection 
initiatively. Because of the performance will be cut down when more than 100 
server connection on it.</p>
<p>Every region cluster consensus efficient in true distributed environment about 
1000 QPS, if user transaction amount proximate 1000 QPS, you need to consider 
add new machine or stratify the trade system. In fact, it is not easy to arrive 1000 
QPS, because of transportation of network. Adding new server to region layer also 
can dissipate trade pressure, the more server we have, the more region we have. 
Normal user is not like machine running pressure test, 1000 QPS require 10 
thousand people to do transaction for it.</p>
<p>Additional, firework block chain allows network system that configures inner 
line as binding IP and outer line as serving IP. We can deploy consensus server into 
container like Docker virtual environment.</p>

## Cache policy

<p>The another fast consensus of firework block chain is that, system put all user 
address nebulous hash and balance cache to memory, and update the cache 
atomically after this user transaction. System support eager, background and none 
cache form. The eager cache mode will cache all nebulous hash before system all is 
ready, the background cache mode will running nebulous caching program after 
system all is ready, this cause all nebulous hash has been cache finally, and let 
system into ready status quickly, the none mode of caching is do nothing on system 
reboot, but will cache nebulous hash after one user do transaction at first time, this 
mode maybe delay request, not every friendly to user, and low performance at start 
phase of server ready, if less data record or huge amount of user, this mode is 
properly, but we need configure working thread of request. System will check user 
how has been idle for long time, and remove its hash from memory.</p>

## Synchronized policy

<p>When server count increase more and more, that is impossible use them as one 
cluster, in this situation, must occur problem of data discord with, one server 
cannot consensus if it present data discord with outer world, unanimous data from 
neither outer world nor consensus by other server it send. We synchronized the 
server data with other server to solve this problem. Firework block chain 
synchronized policy through single thread in background, never expect to modify a 
block chain by multithread.</p>
<p>Furthermore, firework block chain synchronize data by user address, purpose is 
not affect other address when synchronize one address. Firework compare the 
block head whether accord with mostly block head in the cluster, if block head is 
discorded, then update this block with other server data, or validate data root hash 
of this block, go to next if root hash available or fetch the head corresponding data 
from remote host and replace the block. Certainly, system valid any data from 
remote host, and drop them if data invalid or update the block when through 
verification. For safe, server drops the data which not request by itself, only valid 
the data by its request.</p>
<p>It is low and long term in synchronization, but that save system computing 
resources, because it just single thread to do synchronization. Synchronized work 
using a task procession, it is forbidden one address do transaction after it added to 
task procession until its synchronization was completed and been wakeup. System 
change the address to synchronized status when found the address cannot be 
consensus, synchronization maybe cost several ten seconds in pressure testing. The 
reason maybe the NIO thread is front and high privilege and the synchronized 
thread just background thread.</p>

## Transaction contract

<p>Firework block chain using open contract, but need dual customs take part in 
and sign in the transaction to complete trade between digital currency and other 
substantial that has been reckon equivalent by dual customs. Design the ocean 
contract is for connect to other digital currency on the world, we called DOCWTO, 
and make some change for practitioner who want to join in digitalization. 
Meanwhile, the practitioner can grasp business tendency if they deploy transaction
node that can communicate with other node in this digital currency, cause by they 
could do data analysis on their private server node.</p>
<p>Contract transaction proceeds in thirty part server node, firework contract 
transaction reckon dual trust each other, and play a role of bystander. There ought 
to do transaction without exchange private key, be note that, thirty part platform 
show firework token to user for signature postulate that user has will exchange with 
this thirty part, and then they will gain the signature from user and user public key, 
and then invoke consensus service in our system. The service require a token, tow 
signature from dual, public key from dual, exchange amount and one implemented 
ocean contract. After system valid and consensus, the do Trade method will be 
invoke by system for doing private trade in dual exchanger, and commit the 
transaction after private transaction success completed. System broadcast the 
transaction to the world by chain reaction. We recommend synchronize the user 
address before doing transaction.</p>

## High available

<p>High available is the innate property of block chain, but here to explain one 
sample way to do high available, its main scenes is keep interaction with outer 
world without interruption. We can do this by traditional way that deploys tow suit 
of exchange node, but this method not easy to move data and synchronize with 
each other. The other way is deploy a big distributed store system and make tow 
suit of standalone table for tow node. If one node malfunctions, we just clone data 
from another node. This entire table just needs one version.</p>

## Cipher and safety

<p>We are not pretend to make wheels in cipher aspect. Just reuse the TSL which
well-knew on the world, but the certificate are regulating with generic format called 
X509. Its mechanism is generate one secret by random, then cipher real message 
by this secret, and then cipher the secret by RSA algorithm, and transport ciphered 
data and ciphered secret. In safety aspect, we recommend impel user change them 
private key in a fixate time, so that against cracker decipher user private key. 
Besides, this way also can improve user account in a good condition for exchange, 
because if one user chain is too long, that will cost long time to valid the chain 
postulate without first transaction caching. Besides, change the key in timely also 
keep user privacy. There is no man can know who is the user by figure address in 
theory duo to the algorithm irreversible. But if user exposes their address many 
times, maybe bond by manual.</p>
<p>Firework block chain only allow one root block existence, it will valid the whole 
chain of one user before it do transaction if the user has been no cache. Only pass 
the whole chain valid, then allow doing trade and cache them. If any modification 
found in valid it will trigger synchronization. So, the cracker maybe stop a server 
node, tamper data of server is useless, unless change the programing.</p>

## Store system

<p>We recommend use the distributed non-structural and supported cooperation 
processer database, Hbase is a good choice and support standalone for developer. 
We need Hbase big data storage and reading ability, adjust to standalone in 
development phase. Of cause, you can try with other database such as Ocean base 
or even SQLite as store. The table storing block data has one column family is 
enough, and the row key saving blocks head information, column family saving all 
transaction information. We recommend reduce the data that we not really need to 
valid.</p>
<p>In the situation of lacking computing resource, region server amount limited. 
Because the data increment so fast, Hbase configuration maybe need the 
sophisticated engineer to do, or zoo keeper time out phenomenon often occur. 
You had best pre division on block table and optimized the data flush, Hbase is not 
good at data splitting, and that will stop the JVM and throw time out exception and 
kill region server on zoo keeper. Memstore of region server keep default configure. 
And the property of max connections also could consult time out and strike
phenomenon, running in distributed Hbase may be healthier.</p>
<p>The region store file in Hbase is 256M by default, but this is for big data, it 
maybe contains 1000 thousands in a file that size is 256M, that is inimical for
distributed computing, we can adjust it to 128M, so that dissipate the computing 
pressure to other server node. If the block size is small, we can cache them on 
Hbase server, just need to set the family property in-memory to true. Default block 
size is not small enough; about occupy 1.5K space on one record. If you have the 
better verification method, and reduce the space occupation, that will be faster.</p>

## Immortalized solution

<p>By theory, new node initiated status just required saving No.0 user data and 
the target user that we wanted. But all these data chain must be completed. if one 
user address that not conserved in this server node try to trade on this node, that 
will trigger synchronization, so that the new user will been save to the server node. 
By the time going, this server node will has more and more user data. We do that 
just reduce some never has been used data occupy server store space, because old 
data contains many abandoned user chain, these data are useless for new node. If 
we do like that, new node can use any store system including not support 
distributed.</p>
<p>If deploy like that way, should be some node contains lots of transaction data, 
but some node only contains little transaction data. That just like various galaxy 
that in different size and weigh in the university. The big galaxy using by 
cooperation, and the small galaxy using by company. The immortalized solution 
indicated replaces the old node by new node that only contains new data, to keep 
fitness and high performance, we can imagine one’s reincarnation that discard old 
memory and gain a new life. Return to naught and rebuild a new tree.</p>

## Development

<p>Firework block chain was integrated spring boot, and provide one suit of block 
builder, in spring boot programing, developer is easy to define itself block builder, 
the builder define how to build the block and how to verify them, including 
building row key, root hash and hash. That is required verify the data rule according 
how to build them, we can adding some property as big data analysis such as trade 
IP, so that we can know the brunt transaction from where in one phase of time. 
Firework default block builder supported instructed data as block transaction data, 
if we add people identity in transaction, that will supported real name transaction 
limit. In other ways, we can control it if we want. Firework valid data by coprocessor, 
if you override block builder, then must implements the coprocessor and deploy to 
all node of Hbase. The coprocessor contains tow method to implement, one of 
them named ValidRootHash which use to valid root hash on system booting, the 
purpose of valid root hash is prevent data been tamper. Coprocessor another 
purpose is compute nebulous hash and balance of user in distributed system 
environment. It is importance to compute user nebulous hash, user transaction 
consensus base on this hash. That is impossible to sort transaction record in 
different server node, so that cannot compute nebulous hash by transaction order, 
but we can get it by big integer adding and concentrate at one server compute 
again, so that we got the same hash for one user on each start postulate that data 
has not been tampered. We called the hash nebulous hash.</p>
<p>Firework block chain initiative purpose was diminishing difficult for practitioner 
of block chain, so that developer do trade just by http in edge device. But we 
recommend that developer doing the transaction by TCP connection, so that can 
use the computing ability of edge device. All signature just complete by device side, 
server never conserve the private key of user.</p>

## Running environment

<p>We recommend running chain node server in 4+ cores CPU; if the amount of 
node just has few take the default thread configuration is good. But if we have 
many nodes of chain and configure abound connected consensus server, we have 
best configure more threads for server. If we have distributed store, the more 
threads the more user waiting verification at same time, in other ways, we can hold 
more user requests at the same time. And we recommend configure Hbase by 
official instruction and keep health on store layer. If consensus server connection 
less than 10, the server instance not every demanding memory. Several million 
transaction done in pressure test just required 256M-300M, if add the 
transportation memory just about 500M, however, the server which holding upload 
transaction to upper layer chain required a little more in memory. There is (N-1)/N 
delay in time, N indicated number of threads.</p>
<p>We recommend running in 8+ cores hardware if configure many nodes as 
consensus server. The memory usages concentrate on IO transportation and user 
nebulous hash caching. The IO transportation maybe required 256M, 100 million 
users caching required 100M, and the index in Hbase 100 million record required 
200M memory. Firework block chain did not open in memory mode in chain map 
index, because of instance has one layer high cache to against the pressure test, 
and so that low demanding on CUP in Hbase when running pressure test. Open in 
memory mode is fit to real environment.</p>
<p>Firework block chain has a definition of chain map, it use for index transaction 
data. There are two difference implements on it. The first one is caching in JVM 
heap, it is efficient but required memory in node server, the estimate method was 
already toll in previous phrase, and this style of index fit to small or middle server 
node. The second chain map is write index to Hbase, and this demanding Hbase 
configuration.</p>
<p>Software environment, structure developed in jdk1.8+, hbase2.2.2+, 
protobuf2.5 which use for coprocessor development. Recommend running in the 
server system like Linux OS, such as centos support minimum installation.</p>
<p>It is not support disconnect when running pressure test, if one server was 
disconnected, it will be cannot consensus whit other server.</p>

## Bibliography

<p>[0] High transportation framework PhotonIO</p>
<p>https://github.com/Jazping/PhotonIO</p>
<p>[1] China central bank digital currency</p>
<p>https://tech.sina.com.cn/roll/2020-04-23/doc-iirczymi7848983.shtml</p>
<p>[2] Facebook introduces Novi, the renamed digital wallet for Libra</p>
<p>https://www.siliconrepublic.com/companies/facebook-novi-digital-wallet-l
ibra-calibra</p>
<p>[3] Libra 2.0 white book</p>
<p>https://www.8btc.com/media/584947</p>
<p>[4] Battle of international settlement of currency</p>
<p>http://www.xinhuanet.com//globe/2020-01/09/c_138682242.htm</p>
<p>[5] IMF people currency</p>
<p>https://www.imf.org/zh/News/Articles/2016/09/29/AM16-NA093016IMF￾Adds-Chinese-Renminbi-to-Special-Drawing-Rights-Basket</p>
<p>[6] Refectory of global currency by digital currency</p>
<p>http://zhibo.people.cn/watch/5861247</p>
<p>[7] DC/EP vs Libra</p>
<p>https://finance.sina.com.cn/blockchain/coin/2020-05-07/doc-iirczymk035
0707.shtml</p>
<p>[8] Libra and DCEP</p>
<p>https://finance.sina.com.cn/blockchain/roll/2020-04-21/doc-iircuyvh9041
165.shtml</p>
<p>[9] QuarkChain: How Heterogeneous Sharding Empowers Enterprise</p>
<p>https://medium.com/quarkchain-official/how-heterogeneous-sharding-e
mpowers-enterprise-e1ca05131009</p>
<p>[10] QuarkChain. “Boson Consensus: A Scalable Blockchain Consensus 
Algorithm”[Z].</p>
<p>https://github.com/QuarkChain/pyquarkchain/blob/master/papers/boson.
pdf</p>
