# MAnycast² Anycast Census Data Repository
This repository contains the dataset of the Anycast Census (detected /24 Anycast Prefixes), discovered using MAnycast² and validated with [iGreedy](https://anycast.telecom-paristech.fr/dataset/).

<div>
   <table width="100%" height="100%" align="center" valign="center">
   <tr><td>
<img style="float: center;" src="images/ut.jpg?raw=true"/>
   </td><td>
<img style="float: center;" src="images/caida.png?raw=true"/>
   </td><td>
<img style="float: center;" src="images/SIDNlabs_Logo.png?raw=true"/>
   </td></tr>
   </table>
</div>


## Introduction
- Since its introduction in 1993, anycast addressing [RFC1546](https://tools.ietf.org/html/rfc1546) has become a fundamental mechanism to increase the  resilience and performance of Internet services.
- Anycast has been adopted by several cloud providers, Content Delivery Networks (CDNs), and DDoS protection services, among others.
- In a collaboration between UTwente, CAIDA, and SIDN, we proposed a new measurement and inference technique, called MAnycast², which relies on an anycast testbed to efficiently detect anycast prefixes.
- The idea behind MAnycast² is quite simple: We send ICMP echo-requests with our anycast IP address as a source, from all of the anycast nodes in our testbed. The traffic of the ICMP echo-responses to the anycast IP will be then routed back on a single node, if the target is unicast and on multiple nodes, in case the target is anycast.
## Paper
The paper descibing MAnycast² is available here [PDF](https://www.caida.org/publications/papers/2020/manycast2/manycast2.pdf). Reference:
```
@inproceedings{10.1145/3419394.3423646,
      author = {Sommese, Raffaele and Bertholdo, Leandro and Akiwate, Gautam and Jonker, Mattijs and van Rijswijk-Deij, Roland and Dainotti, Alberto and Claffy, KC and Sperotto, Anna},
      title = {MAnycast2: Using Anycast to Measure Anycast},
      year = {2020},
      isbn = {9781450381383},
      publisher = {Association for Computing Machinery},
      address = {New York, NY, USA},
      url = {https://doi.org/10.1145/3419394.3423646},
      doi = {10.1145/3419394.3423646},
      booktitle = {Proceedings of the ACM Internet Measurement Conference},
      pages = {456–463},
      numpages = {8},
      location = {Virtual Event, USA},
      series = {IMC '20}
}
```
## Dataset
|Date       |          Dataset |  # /24 Anycast|
|-----------|------------------|---------------|
|Jan 2021   |    [Jan 2021]()  |            N/A|

## Terms of Use
If you make use of any of the open access data from the MAnycast² project,
you must acknowledge use of this data by including the following attribution
in any document, web page or other communication:
```
"The research leading to these results was made possible by MAnycast²
(https://github.com/ut-dacs/Anycast-Census/), a joint project of the University of
Twente, SIDN, and CAIDA."
```

Furthermore, if you use open access data from the MAnycast² project for
research that is published in a scientific paper, poster or other peer
reviewed content, you must cite the following paper as describing the
method through which the data has been collected:
```
Raffaele Sommese, Leandro Bertholdo, Gautam Akiwate, Mattijs Jonker, Roland van Rijswijk-Deij, Alberto Dainotti, KC Claffy, and Anna Sperotto. 2020. MAnycast2: Using Anycast to Measure Anycast. In Proceedings of the ACM Internet Measurement Conference (IMC '20). Association for Computing Machinery, New York, NY, USA, 456–463. DOI:https://doi.org/10.1145/3419394.3423646
```
We keep track of research papers that use data from MAnycast² on this website,
and would appreciate it if you can notify us of any publications in which you
use our datasets. Please contact r.sommese@utwente.nl and
a.sperotto@utwente.nl, and send us the citation of you paper.
