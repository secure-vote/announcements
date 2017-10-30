# SecureVote: Addresses and Protocols

This concerns the Ethereum contracts, addresses, ENS names, and protocols SecureVote will use when conducting end to end verifiable ballots via Ethereum and other platforms.


## Announcements

Firstly, all announcements will be made in a cryptographically secure way via Ann.sol - a smart contract for managing announcements containing cryptographically sensitive information. It integrates ENS and announcement auditing in a way that makes fraudulent announcements near impossible.

You can find details of Ann.sol at our repositories:
* https://github.com/secure-vote/ann.sol/
* https://github.com/secure-vote/ann-sol.com


## Our Addresses and ENS names

Secondly, here are the current Ethereum addresses and their ENS names used by SecureVote

* secvote.eth: 0x0Db4DC6E5A9039b2b8fCA026963655B04596E903
  * this is an overall management key

* ann.secvote.eth: 0x7B7f585506f997859811e527A4bF44e34363eD77
  * this is the smart contract by which this announcement is made secure

* deploy.secvote.eth: 0xE8193Bc3D5F3F482406706F843A5f161563F37Bf
  * this is our address from which we deploy voting smart contracts


## Protocols around votes run on Ethereum

Although SecureVote is building a high capacity chain build specifically for voting, from time to time we will run ballots over the Ethereum network.

When this occurs, two things will occur:

* All ballot smart contracts will be deployed from deploy.secvote.eth
* Every such smart contract will be given a secvote.eth ENS subdomain

This subdomain will be of the form <short-description>-<date>.secvote.eth

e.g. swarm-trs-nov-2017.secvote.eth


## Future plans

In future we will have a ballot-specific smart contract for announcing upcoming ballots and their ENS domains, to be integrated within the upcoming SecureVote app.


## Conclusion

In conjunction these protocols and structures will ensure all ballots conducted by SecureVote are not only end to end verifiable in and of themselves, but also announced and maintained in a cryptographically secure way.

As leaders in the digital election space we feel these measures are the minimum required to give voters they assurance they deserve.


LLAP,
Max Kaye
CTO, SecureVote
