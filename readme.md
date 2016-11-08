![N|Solid](http://i.imgur.com/LLRzEbF.png)

# Proof: A Cross-Blockchain Contract & Asset Management Platform





Proof is an agnostic, trustless system for transmitting information across multiple distributed ledgers, better known as “blockchains”. This solution allows digital agreements, cryptocurrencies, and digital assets to move between parties using different ledger types, managed via a decentralized application and synced via a sidechain. Specialized smart contracts, computer nodes, or a combination of the two designed for particular blockchain types serve as orchestrated oracle systems on top of participating blockchains, following a common standard for seamless synchronization of aggremement execution and asset recordation. This solution also relies on an easy-to-use interface which allows non-technical users to manage their land deeds, financial accounts, intellectual property holdings, identity, legal agreements, and other assets, taking advantage of the underlying trustless infrastructure.




	
# Introduction


Administration of rights, agreements and ownership of assets currently consists of fragmented processes, especially when participating parties reside in or are different institutions or exist in different legal jurisdictions. Often times, transfer of asset ownership occurs on government-regulated exchanges or between licensed brokers while expensive settlement processes must finalize deals and administer certificates or funds involved in transactions. Currently, financial institutions and other organizations are introducing blockchain technologies in order to solve the problem of settlement upon transaction.  While Visa leverages technology provided by Chain for fund transfer, Nasdaq is currently leveraging Chain technology for the trade and settlement of over-the-counter stock trades, and The Japan Exchange Group has begun experimenting with IBM’s Fabric blockchain. While the blockchain solutions of these companies solve settlement and trade latency issues, they do not address the fragmentation of asset ownership certification information.


When the creator of intellectual property licenses rights to an organization, royalty payments and any disputes arising from the agreement are part of a decentralized process that often can be expensive and fraught with error.  These errors can arise from human error or poor information management.


In another case, insurance policies are often traded in tranches between insurance firms in a process called reinsurance. When insurance claims are created by the insured and payment issued, settlement between the many firms who possess the risk associated with partial ownership of a policy can be a time-consuming process.


Smart contracts are a means to solve many of these issues, by holding or accessing funds, or transferring ownership rights autonomously based on pre-determined, agreed upon, conditions. These smart contracts leverage the cryptographic proof benefits of blockchains and often cannot be altered after creation, providing an objective interpretation and administration of those agreements.


However, as many platforms have emerged for hosting smart contracts, such as Ethereum, Eris, and Fabric, fragmentation can cause conflicts across different systems, with records of assets existing potentially on multiple chains, creating an issue for settlement and accurate accounting.


The proposed solution consists of a platform that communicates with and transfers assets between these different blockchains, leveraging their cryptographic proof of validity and immutability.  The solution will also allow anyone to monitor, create and manage rights, assets and currency.  Furthermore, a user interface allows for easy adoption by both technical and non-technical individuals and institutions who desire to confidently prove ownership, transfer ownership, and perform other activities in a universally accepted fashion.




# Digital Assets on Blockchains


	 	 	
Ownership of a physical or virtual assets is recognized by a record, usually in a government database. Today, these databases are often centralized and access to these records can sometimes by costly or depend on some sort of clearance. Additionally, motor vehicle ownership records and stock ownership records are often contained in spate databases, either on paper or in digital form in different departments of governments. 


When an owner would like to transfer ownership, there are often a few intermediaries, conditions and fees one needs to satisfy in order to make that transfer officially recognized by a government organization. Overstock, a publicly held company, received permission from the Securities and Exchange commission of the united states to represent their ownership stakes and transfer that ownership using the distributed ledger technology of Bitcoin. In Georgia, land ownership is now partially maintained using distributed ledger technology.

Private institutions often have the right to transfer ownership of financial assets between one another privately. Many institutions have to record ownership of financial assets on distributed ledgers in order to leverage distributed consensus models to prove ownership. As more companies, governments and individuals record and recognize ownership using blockchains, it is important that the cryptographic proof of ownership can be maintained between distributed ledgers.


This is addressed and a process was introduced in a whitepaper entitled “enabling Blockchain Innovations with Pegged Sidechains” by Asam Back et al. However, smart contracts and the rights of ownership and other conditions contained within them must be considered in addition to currency and digital inputs of transactions. Smart contracts contain conditions and execute trades based on those conditions within virtual environments of blockchains such as Ethereum and Eris. These more complex transactions based on agreements must communicate with other smart contracts in order to move transactions between chains.






# Computer Nodes


Computer nodes connected to blockchains perform the roles of validating transaction, submitting new transaction, and reading existing transactions. As validators of transactions, typically a node will check that blocks, or collections of transactions contain headers, or information, stemming from a previous transaction, and that those previous transactions do the same. This is the nature of a blockchain that ensure the append-only nature of a blockchain. In doing so, they serve as a mechanism that decentralizes trust that a transaction is valid, and that inputs from one transaction cannot be used in a separate transaction, or “double spent”.


As submitters of transactions, computer nodes leverage the proto of a particular blockchain to communicate with the rest of the network, submitting hashes of transactions to be included in upcoming blocks that are to be validated by the network.


As readers of transaction, the nodes have access to previous transactions for the purposes of both relaying valid transactions and validating them. In the purposed system, computer nodes would accept information from a distributed software application connected to outside blockchains, interpret them into transactions for the blockchain they exist on, and submit them. Additionally, these nodes would accept requests to transfer a transaction from their current blockchain to the distributed application, which then communicates that transaction to another node on a different blockchain.




# Scopics


Scopics, or Smart Contracts On Permissioned Immutable Computers, are mechanisms that can exist on permissioned or public blockchains and perform execution based on predefined conditions. Permissioned blockchains are not public and often rely on trust between parties within the blockchain to reach consensus regarding a transaction, while public blockchains are trustless and rely on consensus of a majority of nodes on the network.
For the proposed solution scopics operate by leveraging a common protocol that can accept input from smart contracts on a particular blockchain and interpret them in a way that locks certain assets contained in those contracts so that they can corresponding computer nodes can orchestrate the transfer one asset from blockchain to blockchain.




	
# Blockchain Transfer Protocol

Figure 1

![N|Solid](http://i.imgur.com/eOf1Znw.png)

Figure 1 depicts how a user might transfer an asset from one blockchain to another, when an asset is transmitted from a blockchain that does not have smart contract capabilities. This figure also demonstrates how those assets might be unlocked and used later by another user on the originating blockchain. The arrows are numbered to demonstrate the flow of a possible set of transactions, as the asset moves from identity to identity. 
In step 1, the originating user, sends assets to an Proof generated address. In steps 2 thru 3, The DAD is monitoring information of generated addresses and once the address confirms receipt of the transaction, the DAD then sends a representation of the asset to another blockchain, while copying the transaction to its sidechain.
In the proposed solution, that user can then transfer the asset within their own permissioned chain, and then a user can send the asset back to the originating chain. When this is done in step 4, a transaction is crafted using the secured key of the created address to send funds to the destination user at the bottom of the diagram. This transaction is also stored on the sidechain.

When an asset or contract is transferred from one blockchain to another, a common protocol must be shared.  This allows the same asset to be transferred back to the originating chain and moved from there. To accomplish this, the private key or other credentials need to access the locked funds in the originating transfer address controlled by the proposed solution’s node and then access the holding address and transmit the asset in question.


The proposed solution includes a distributed software application with a corresponding database that holds the private credentials of addresses that hold funds or other assets moved to another chain. Simply encrypting these keys or credentials in vulnerable to an attack which can expose the key and cause a “double spend” of the a particular asset. To prevent this, the private key of an asset is stored across several locations with several keys to unlock the key. For a key of a holding address to be unlocked, consensus must be created within the distributed application that the owner of an asset would like to transfer that asset back to the originating chain.  The asset will then transfer along with a parameter stating which address that asset should be transferred to.
The protocol used specifies the “holding address” that the asset is transferred to, the chain to and from the asset is to be transferred between, the originating transaction hash that the transaction originated from, and a special hash generated by the software application moving these funds. This special hash represents the hash on the external network that was created when the asset was created on an alternative chain.


# User Interface


The user interface of the solution entails a menu consisting of several tabs including: my assets, my transactions, organizations, multi-blockchain explorer, and settings.
My assets consists of accounts and smart contracts to which a user owns or is participating in, with an overview of the balances, assets, and conditions of smart contracts, whether in natural language or existing in code in the form of a smart contract.


My Transactions consist of transactions pertaining to assets to which are under control or of which an individual is participating in. It can also consists of transactions to which an assets the user is currently monitoring.


Organizations consists of a search of other identities and the current organizations a user has joined by permission of a particular organization.


The multi-blockchain explorer consists of a record of public blockchains that the Proof has a node on, or if the blockchain is a private one, where or not a user has access to view along with the required conditions for access.    The explorer also allows the user to navigate through different transactions and view the state of smart contracts a user is tracking. 


Settings contains the visibility options for a user, allowing them to create and trade assets anonymously or semi-anonymously.  It lists transactions user is participating in, their name, email and other personal details.


Within the my assets tab, a user can create an asset on a blockchain and manage it. If it is a cryptocurrency, the user must send funds to a generated address to track said asset.  In my transactions, a user can perform function of a asset, such a send it, or in the case of a smart contract, a user can access the different methods available to that user within the contract such as edit a particular state.



![N|Solid](http://i.imgur.com/QX9jgWP.png)

Figure  2 depicts an Proof portal user interface. In this mock-up, a user is shown creating a transaction to move a 50 bonds of HK Corportation stored on a public blockchain to an identity on a permissioned blockchain.






# Distributed Software Application


Proof’s Distributed Application on Decentralized DNS (DAD) unifies these systems by connecting to Scopics which then act as oracles to legislate transactions and operate from an easy-to-use interface for placing/modifying/managing assets across multiple chains by people with differentiated technical expertise.  After transactions have completed, the DAD reads the final transaction and creates a record on a side-chain which allows for fast interactions and solid record keeping.

The DAD handles a cryptographically secure database of private keys which allow for the seamless movement of assets across multiple chains, allowing assets deployed across many chains to interact and be traded.  

An asset’s existence will be initiated by a user who can be an institution, an individual, or a proxy acting on behalf of either. User interaction with the underlying system will be handled by the UI with all actions on an asset  being recorded and handled by the DAD’s underlying protocol. 

The DAD protocol will have a dual layer verification scheme consisting of payment verification and transaction verification.  For payment verification, Proof will check that actions on the parent chain successfully occurred using a standard Simple Payment Verification (SPV) proof such as the broom filter [A] or the proposed Ethereum Light client.  Second, before sending, the Proof builds and formats transactions insuring solid interoperability between blockchains. 


The DAD also holds any keys or authentication information in an encrypted format in order create transactions and verify identity to scopic oracles.  Initially, the encrypted storage will resemble the implementations laid out in Storj’s MetaDisk white paper.


Similarly, the DAD will monitor the movement of transactions on the to-chain as assets move there, maintaining a snapshot of the asset’s state and location inside of a merkle tree.  The two-way integrity of this data will be verified by TLS Notary.  

Since interoperability is a primary goal of the entire system, the DAD system can potentially contain protocols for all of the major public and private blockchains including Bitcoin, Ethereum, Eris, Hyperledger Fabric, Chain, Dragonchain, Dash, and Ripple.  Expansion to any other asset chain, such as a bank’s private blockchain, will be supported with the cooperation of involved parties.  Likewise, for blockchains supported by a digital currency, actual value can be transmitted to users and entities.   


Scopic are essential for the Proof DAD system.  Scopics act as intermediaries between the DAD, ‘to’ chains, and ‘from’ chains.  The scopic stores the address locations for assets on each chain while also performing the transactions on the chains.  The Scopics could be considered ‘oracles’ for the asset’s existence.  Each scopic manages the asset’s movement while holding funds and ensuring that an asset cannot be double-spent while keeping an immutable record of the transactions.

The sidechain consists of blocks containing a record of each transaction run by the Proof.  In a sense, it is a lightweight, chain-agnostic, implementation of the bitcoin sidechain protocol mentioned above.  The Proof Sidechain is based on the Ethereum blockchain which in turn is based on Bitcoin.  Written into blocks secured by a Proof-of-Work system, side-chain data will consist of the chain type of each interacting chain, the asset name and type, the two addresses on each chain, and the two addresses of the oracle scopics where the asset was both taken from and placed.  The side chain acts as a record of scopics and inter-scopic transactions  while the scopics act as records of transactions between the oracle scopic and the blockchain on which it is deployed.




# Demonstration of DAD

![N|Solid](http://i.imgur.com/rCUdS6J.png)

Figure 3 demonstrates how an asset in token form or input in cryptocurrency form can be transferred between smart contract-enabled blockchains. The diagram is split into 4 sections (from upper-left in counter-clock-wise or): 


The user initiating a transaction on the Proof platform
The Proof sidechain for tracking external blockchain information for tokens and currency moving between different blockchain 
The originating blockchain of the asset in question, in this case similar to the Ethereum public blockchain
The destination blockchain, in this case, a permissioned blockchain similar to a IBM Hyperledger Fabric chain.


To depict the process, numbered arrows are presented and can be described as follows:

  1.  The user leverages his/her identity connected to their private credentials (such as a certificate, key, or other authentication mechanism) to request that 20 ether be sent from the ethereum  blockchain to a permissioned blockchain for a merchant.
 
  2.  The Distributed Application on Decentralized DNS (DAD)  checks that the transaction is valid and formats the transactions to be broadcasted on the Ethereum network, using the user’s credential. The DAD then broadcasts that transaction to the ethereum network, sending funds from the user’s account to account.
  3.  The transaction created by the DAD sends funds to a smart contract serving as a locking address for the funds and also an oracle for the DAD network, serving as a ledger for fast search capabilities. 
  4.  The DAD queries the smart contract to check for funds confirmation. Once the funds confirmation is affirmed on the Ethereum network.
  5.  Once the DAD reads and verifies the destination details from the scopic on the Ethereum network, it creates a transaction on the Proof sidechain, a fork of the Ethereum blockchain, which contains an immutable list of transactions between chains, with details of destination address with the writes to transmit it further or back to the Ethereum chain.
  6.  Once the transaction is saved on the sidechain, a representation of the asset is crafted on the Permissioned Fabric chain, thus the asset has thus moved from the Ethereum network to the Fabric network, with verification and transaction hashes saved on the sidechain.






	

# Financial Instrument Use Case


*Mutual funds, ETFs, brokers, investors, ecosystem description. Explanation of where benefits of blockchain arise from : Settlement upon trade, consensus regarding transactions, consensus among credit and reputation information, pre-correctness
```javascript
contract asset{
    
    ...
    //standard token vars
    string public standard = 'Token 0.1';
    string public name;
    string public symbol;
    uint8 public decimals;
    uint256 public totalSupply;
     modifier onlyOwner {
        if (msg.sender != owner) throw;
        _
    }
    //balances stored here:
    mapping (address => uint256) public balanceOf;
    //IP info
    public string content ="All of the users content to be copyrighted";
    public address owner  = 0x6358272727812781; //Creator's Address
    function asset(){
        ...
        //intellectul prop start info
    }
     function transfer(address _to, uint256 _value) {
        if (balanceOf[msg.sender] < _value) throw;           // Check if the sender has enough
        if (balanceOf[_to] + _value < balanceOf[_to]) throw; // Check for overflows
        balanceOf[msg.sender] -= _value;                     // Subtract from the sender
        balanceOf[_to] += _value;                            // Add the same to the recipient
        Transfer(msg.sender, _to, _value);                   // Notify anyone listening that this transfer took place
    }
    function transferOwnership(address newOwner) onlyOwner {
        owner = newOwner;
    }
    function createRightOrSupply(int creationInt) onlyOwner{
        totalSupply = totalSupply + creationInt;
        ..optionally defined details regarding supply... if intellectual property, detail... if non-intellectual property, then increate supply
    }
}

```


# Financial Instrument Use Case

Financial Instrument transactions included exchanges and issuance of bonds, insurance policies, company shares, derivitives, and packages composed of a collection of each. Each of these asset classes can be represented using a token contract on a smart contract-enabled chain or via the Open Asset Protocol. When an institution issues a loan, they effectively exchange currency or highly liquid asset on the blockchain for tokens composed of units aligning with the interest and other agreements set forth in a contract template for the particular kinds/terms of the asset class. These tokens can be exchanged between instituions. A user issues repayment for their bods with interest to the token smart contract, which delegates ownership to holders of cooresponding tokens. A similar case can be used to prove ownerships of shares, packages, and other assets using these token, and recieve benefits, such as dividends in the case of stocks. The benefit of using smart contracts on top of interoperable blockchain's via the proposed solution is for simultenous settlment upon trade, as well as assurance of compliance and legal recognition granted via immutable agreements templates that make the issuances possible. 

# Intellectual Property Use Case

When a content creator produces their work, a submission is submitted to the user's desired blockchain as data in a transaction. From there, the user leverages the solution's protocol to create rights which can be transferred via a template of the user’s creation via the platform to transfer licenses and ownership. 


The transfer of ownership is represented via the desired smart contract. If a user submits a submission to a blockchain which does not support smart contracts, the user can use the Open Asset protocol, also called a “colored coin”, to represent the the shares of such a creation. This asset can be tracked via the inputs of this transaction to other users via the nodes, smart contracts, and other ecosystem tools to other blockchains as described previously.


A user can then track licensing agreements and receive funds to the desired address based on smart contract predetermined agreements,



# Real Asset Use Case


Proof can monitor and manage the manufacture and distribution of a physical asset from the beginning of its existence to its eventual scrapping.   For instance, a manufacturer can take a newly created automobile, place the parts, model number, timestamp, and title on a blockchain using the Proof.
After the manufacturing phase, the vehicle can then be tracked as it moves through the entire supply chain with addendums and compliance notes added to the Proof record.

Along with record keeping, the Proof Scopic system can also hold asset transfer based on the needs of the transaction.  For instance, if the vehicle needed emissions checks before entering the market, a government regulator could check the car for standards compliance and not until the model had been verified as emissions compliant would it be transfered to a dealer.  This compliance process could be integrated into any level of the Proof chain of ownership, including placing holds on manufacturing, sales, or leasing.
 
# Implications for Government


The Proof is a system that will allow governments to go completely paperless with full confidence and ease.  The largest hurdle for blockchain's broad adoption, especially for governmental employees who must have an encyclopedic knowledge of regulations and processes while also juggling operations, is the high barrier to entry due to technical complications.  The Proof simplifies this by adding a user-friendly interface on top of a robust, chain-agnostic engine.   

Since all assets, locations, and transactions on blockchain can be tracked, Proof will cut down on required time, increase reliability, and reduce the cost of compliance and organizational resource distribution.  With countries and cities such as Dubai and the government of The United Kingdom investing billions into blockchain technology, Proof expedites the process of adopting blockchain into processes such as internal asset transfer, voting, and record keeping.  





# Implications for Enterprises



For enterprises, the Proof will reduce time for inter-organizational asset transfers.  With its easy-to-use interface, the amount of time necessary to train employees on the software will be minuscule, and with the DAD system in place, asset transfers between companies will be simplified.  This will eliminate the need for costly ad hoc solutions and side chain deployments by enterprises.  
	
In the future, the inbuilt tracking mechanisms of Proof will lower costs for auditing and make compliance a much simpler process for both governments and enterprises reducing legal fees for corporations and businesses.

As companies such as VISA expand on their Business-to-business blockchain offerings, Proof will become an essential solution for fast deployment and asset transference on blockchains.     

VISA’S b2b platform promise to lowering of costs for auditing, investigations, and compliance and legal fees.

	
# Implications for Consumers


Why consumers benefit and how they can protect themselves in the case of insurance and other areas where trust will rely less on institutions and ability to take control of their assets, agreements, etc. and also purchase and use them in more informed fashions, making the entire ecosystem of the aforementioned entities more efficient.




# Road to Adoption


Widespread adoption of this solution of standardization among ownership, rights and agreement mechanisms between blockchains requires 3 areas of focus. These areas include:

- Development
- Testing
- Integration
	
# Government Working Group and Industrial Consortium collaboration


Currently, there are consortiums forming around the world, from R3’s 80+ global banking consortium, to China’s government blockchain working group, to the U.S. fintech research office in Washington. It is important for these organizations to share information regarding research , development and implementation, as well as business challenges and proposed solutions. It will be important for blockchain news and research aggregation mechanisms to be in place that allow researchers and practitioners to share their finds either publically or privately within relevant networks.
	
# Open development and technical collaboration

In regards to solution development, it will be important to have the underlying distributed software package open-source so that as many nodes as possible can work ro ensure the integrity of the system. Furthermore, additional development and more eyes from around the world working on the project, penetration testing it, etc. will ensure maximum security, trust scalability, and software improvements/maintenance.


# Strong, easy-to-understand, multi-lingual and free educational material distribution


To gather “buy-in” from necessary government agencies and large enterprises to recognize blockchain technology for consumer and other institutions/government to deal in to make the asset and contract management processes more efficient, great content that can drive home the use cases and make how to use the software system. This will include short video content centered around royalties, licensing, asset management, stock purchases, content monetization, and other use cases. The first step to adoption is explaining why distributed, yet standardized mechanism for asset and contract management is import. This document strives to be one of many steps to move us closer to wider acceptance of this belief.

# Bibliography

1. [Bitcoin Whitepaper by Satoshi Nakamoto](https://bitcoin.org/bitcoin.pdf)
2. [Sidechain whitepaper](https://blockstream.com/sidechains.pdf)
3. [Token Standard on Ethereum](https://www.ethereum.org/token)
4. [Hyperledger specification documents](https://hyperledger-fabric.readthedocs.io/en/latest/)
5. (Graphics) [IBM and Blockchains](http://www.ibm.com/blockchain/what_is_blockchain.html)
6. [Rule-based XML Mediation for Data Validation and Privacy Anonymization](http://ieeexplore.ieee.org/document/4578505/)

# Contributors

- Mike De'Shazer
- Tai Kersten
- David Van Isacker

