# BitCoin-Generator-SCALA
Generated BItCoins in SCALA!

There are two files: 'Server' and 'Client'
Here 'Server' acts as your master and 'Client', your Worker
The steps to execute them are as follows:
  1) Create separate projects for the Server and the Client programs in the Eclipse IDE for Scala.
  2) Run the Server and pass the necessary argument which is the value of 'k'.
  3) Immediately after, run the Client program and pass the necessary argument which is the IP address of the server.

The following result was tested on Windows OS, one i5 processor of 4 cores and another i5 processor of 2 cores.
Time was measured in the unit of seconds.

1)We determined results for work units of 2000, 8000. Here, work unit is the number of input strings for which Bitcoins were mined.

For 2000 input strings the performance were as follows:

Actor       No. of Bitcoins    Time Taken     Work Units

MASTER      200                24             1000

WORKER      220                22             1000

For 8000:

Actor       No. of Bitcoins    Time Taken     Work Units

MASTER      938                123             4000

WORKER      926                117             4000


While printing the Bitcoins, the ones mined by the Worker are printed in the format: "Bitcoin" \t "UFID+Random String".
The ones mined by the Master are printed in the format: "UFID+Random String" \t "Bitcoin"

2) On running the code with k = 4, managed to mine 29 Bitcoins in a duration of 82 seconds. The result file (output_4.doc) has been included in the project zip.

3) With k = 5, there were 3 Bitcoins with a duration of 10 seconds.

4) The coins with the most 0s we managed to find were: 

spandu1011eS9XtD1JhX : 000006ce20f63f0885cb908ba83c5507bdb05627a40213bfeb5f93ae0e63b852
spandu1011W4T1jd1jxZ : 000006ce20f63f0885cb908ba83c5507bdb05627a40213bfeb5f93ae0e63b852
spandu10116NNZFH68d2 : 000002063b59eceb5d8d135ff9381ae5ae3a3dba6c6659f2c96eccfa3e40bcc8

5) We were able to run the code on 2 machines.

References:

http://doc.akka.io/docs/akka/2.2-M2/scala/remoting.html
http://doc.akka.io/docs/akka/2.0/intro/getting-started-first-scala.html
http://www.scala-lang.org/documentation/
