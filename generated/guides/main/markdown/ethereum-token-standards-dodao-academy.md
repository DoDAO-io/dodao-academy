## Ethereum Token Standards


## Introduction


## Summary

On token interfaces, a lot of Ethereum development standards are focused. These standards aid in maintaining the composability of smart contracts, ensuring that, for example, when a new project releases a token, it is still compatible with the decentralized exchanges that already exist.


## ERC Token Standards

Ethereum Request for Comments (ERC) is a document that smart contract programmers use to create smart contracts on the Ethereum blockchain platform. These publications specify the requirements that Ethereum-based coins must meet. On token interfaces, a lot of Ethereum development standards are focused. These standards aid in maintaining the composability of smart contracts, ensuring that, for example, when a new project releases a token, it is still compatible with the decentralized exchanges that already exist.

    


---
## Popular Token Standards - Part 1



## **ERC-20:** 
The ERC-20 token standard is a guide for developing fungible tokens on the Ethereum network. A token (or a portion of a token) must be fungible in order to be equal to and interchangeable with other tokens.

A coin must support all of the functions and events defined by ERC-20. Remember that this standard also controls smart contracts for newly minted tokens' activities. The bare minimum requirements for features and data in an ERC-20 compatible token are:

### Functions used:

1. `function name() public view returns (string)`
2. `function symbol() public view returns (string)`
3. `function decimals() public view returns (uint8)`
4. `function totalSupply() public view returns (uint256)`
5. `function balanceOf(address _owner) public view returns (uint256 balance)`
6. `function transfer(address _to, uint256 _value) public returns (bool success)`
7. `function transferFrom(address _from, address _to, uint256 _value) public returns (bool success)`
8. `function approve(address _spender, uint256 _value) public returns (bool success)`
9. `function allowance(address _owner, address _spender) public view returns (uint256 remaining)`

### Events are:
1. `event Transfer(address indexed _from, address indexed _to, uint256 _value)`
2. `event Approval(address indexed _owner, address indexed _spender, uint256 _value)`

## **ERC-721:** 
ERC-721 is a token standard for non-fungible tokens (NFTs). Non-fungible tokens are a special type of cryptographic token that cannot be mutually interchangeable because of their individual specification. This means that 1 token cannot be exchanged for another due to its unique specifications.

An ERC-721 Non-Fungible Token Contract is one that implements the functions and events listed below. Once it has been deployed, the contract is in charge of managing the tokens that have been produced on Ethereum.

### Functions used:

1. `function balanceOf(address _owner) external view returns (uint256);`
2. `function ownerOf(uint256 _tokenId) external view returns (address);`
3. `function safeTransferFrom(address _from, address _to, uint256 _tokenId, bytes data) external payable;`
4. `function safeTransferFrom(address _from, address _to, uint256 _tokenId) external payable;`
5. `function transferFrom(address _from, address _to, uint256 _tokenId) external payable;`
6. `function approve(address _approved, uint256 _tokenId) external payable;`
7. `function setApprovalForAll(address _operator, bool _approved) external;`
8. `function getApproved(uint256 _tokenId) external view returns (address);`
9. `function isApprovedForAll(address _owner, address _operator) external view returns (bool);`

### Events are:



1. `event Transfer(address indexed _from, address indexed _to, uint256 indexed _tokenId);`
2. `event Approval(address indexed _owner, address indexed _approved, uint256 indexed _tokenId);`
3. `event ApprovalForAll(address indexed _owner, address indexed _operator, bool _approved);`

    


---
## Evaluation





##### Why are ERC Token Standards used?  
     
- [ ]  it is the name of a token
- [x]  use to create smart contracts on the Ethereum blockchain platform
- [ ]  for categorizing tokens
- [x]  to ensure smart contracts are compatible in the whole ecosystem





##### Which of the following statement is incorrect?  
     
- [ ]  ERC-20 token standard is used developing fungible tokens on the Ethereum network
- [ ]  functions and events are requirements to make ERC-20 and ERC-721 tokens
- [x]  Non-Fungible tokens are mutually interchangeable
- [ ]  ERC-721 is a token standard for non-fungible tokens

    


---
## Popular Token Standards - Part 2

## **ERC-777:** 
ERC-777 is an improved version of the ERC-20 token standard. It addresses the limitations of ERC-20 by making it more efficient for smart contracts to send and receive tokens. This is done through a mechanism known as ‘Hooks’. Hooks is a function that combines two messages - sending tokens and notifying a contract - into one. In addition, the ERC-777 also introduces the ability to reject transactions from a blacklisted address.

 A smart contract's code describes a function called hooks. When tokens are sent or received through the contract, hooks are called. This enables a smart contract to respond to tokens coming into or going out of it.

## **ERC-1155:** 
A common interface for token management contracts that handle various token kinds. Any mix of fungible tokens, non-fungible tokens, or other configurations may be used in a single deployed contract (e.g. semi-fungible tokens).

The goal is to develop a smart contract interface that can represent and manage any number of fungible and non-fungible token kinds. The concept is straightforward. The ERC-1155 coin can thus do the same tasks as an ERC-20 and ERC-721 token, and even both simultaneously. The best part is that the ERC-20 and ERC-721 standards have improved functionality, efficiency, and correction of glaring implementation flaws.

## **ERC-4626:** 
The ERC-4626 standard was created to optimize and unify the technical parameters of yield-bearing vaults. It provides a standard API for tokenized yield-bearing vaults that represent shares of a single underlying ERC-20 token. The optional extension for tokenized vaults utilizing ERC-20 offers basic functionality for depositing, withdrawing tokens, and reading balances.

Lending markets, aggregators, and intrinsically interest-bearing tokens help users find the best yield on their crypto tokens by executing different strategies. However, these strategies are often done with slight variations that can lead to errors or waste of development resources.

ERC-4626 in yield-bearing vaults will lower the integration effort and unlock access to yield in various applications with little specialized effort from developers. This will create more consistent and robust implementation patterns.


    


---
## Evaluation





##### What is the use of 'Hooks' in ERC-777?  
     
- [x]  Through hooks, a contract can get tokens and be notified in a single transaction
- [ ]  They are used to create a token
- [ ]  They are used to specify the total supply of tokens
- [ ]  They are used to specify the owner of the token





##### How is ERC-1155 different from ERC-20 and ERC-721?  
     
- [ ]  ERC-1155 is a standard for NFTs only
- [ ]  it prevents fund loss
- [x]  both fungible tokens and non-fungible tokens can be created from a single deployed contract
- [ ]  ERC-1155 makes token transfer easy





##### What statements are correct regarding ERC-4626?  
     
- [x]  It optimises and unifies technical parameter of yield bearing vaults
- [ ]  It is used for renting out your NFTs
- [x]  It will reduce integration efforts for developers
- [ ]  It is used in transferring fungible tokens

    


---
## Other for Fungible Tokens

## Other Standards for Fungible Tokens

* **ERC-1404:** The ERC-1404 consensus allows token creators greater control over token circulation and user visibility. The token differs from the typical ERC-20 standard frequently applied to altcoins by having the ability to identify holders of the token and freeze supply. 
* **ERC-223:** Token contracts and contracts working with specific tokens can implement standard functions described in ERC-223 to prevent unintentional token sends to contracts and make token transactions behave like ether transactions.
* **ERC-667:** The ERC-677 standard aims to provide additional functionality without overriding the existing ERC-20 standard. This standard adds a new function, transferAndCall(), which is unlike the ERC-223 standard, which overrides the existing transfer() function.
* **ERC-1203:** The Standard interface for a token contract with multiple token classes is also ERC-20 compatible, which makes it an ideal solution for those looking to use a variety of tokens within their application or system.

    


---
## Other for Non-Fungible Tokens

## Other Standards for Non-Fungible Tokens
* **EIP-5114**: Soulbound Badge was first proposed in 2019 by the Ethereum
  developer Eric Conner, and is currently in the process of being reviewed
  and discussed by the Ethereum community. Some of the key features of
  EIP-5114: Soulbound Badge include:
  
    1. Unique digital assets: EIP-5114: Soulbound Badge allows for the
    creation of unique digital assets that cannot be replicated or divided,
    providing a strong foundation for applications such as collectibles and
    gaming assets.
    
    2. Secure ownership: EIP-5114: Soulbound Badge includes built-in
    mechanisms to ensure that the ownership of soulbound badges is secure and
    cannot be transferred or stolen.
    
    3. Flexible token behavior: EIP-5114: Soulbound Badge allows for the
    customization of the behavior of soulbound badges, including rules for how
    they can be transferred and other aspects of their functionality.
    Overall, EIP-5114: Soulbound Badge is seen as a valuable addition to the
    Ethereum ecosystem, providing a strong foundation for applications that
    require unique, non-fungible digital assets. If adopted, it could enable
    the creation of a wide range of new applications and use cases on the
    Ethereum blockchain.

* **ERC-809:** The standard for renting out your NFTs, is by creating an API to allow any “rival” NFT to be rented. An NFT is considered rival if being in possession of the NFT simultaneously prevents consumption/access to other individuals. ERC-864
* **ERC-1190:** The ERC-1190 token will allow the creators of unique digital objects, such as a work of art or an object in a game, to benefit from the use of those objects over time. This means that even if the object is not used for a long period of time, the creator will still receive compensation for its use.
* **ERC-1238:** ERC-1238 is the standard for Non-transferable tokens that represent "badges". A badge is a token that, once given, cannot be changed. Over time, badges can accrue and be put at risk. In a nutshell, badges are declarations about a public key; they might be qualitative or quantitative (e.g., reputation, experience) (badges, titles).
* **ERC-994:** Delegated Non-Fungible Tokens, or DNFTs, are a proposed extension of the ERC721 standard that aims to provide a way to register land and physical property on the Ethereum blockchain. NFTs are arranged in a federated, tree-like format (similar to DNS), allowing NFTs to delegate and sub-contract other NFTs within a certain geographic area.
* **ERC-998:** The standard extension for a non-fungible token is to own other non-fungible ERC-721 or standard fungible ERC-20 tokens. This means that the entire hierarchy of items is transferred when the token composition is transferred.

    


---
## More Standards


## Standards for Transferring tokens
* **ERC-965: **The aim of this proposal is to allow for pre-signed messages that would enable third parties to execute a token transfer without the original sender needing to do an on-chain transaction. The sender would need to sign a message and the third party would call sendByCheque() with the signature. This would save the sender time and effort in having to do an on-chain transaction.
* **ERC-865: **This proposal outlines a standard function that a token contract can implement to allow a user to delegate the transfer of tokens to a third party. The third party would be responsible for paying the gas fees associated with the transfer, and would also take a small fee in tokens as compensation.
* **ERC-995:** The ERC223 standard provides an augmented token transfer functionality that goes beyond the legacy ERC20 functionality. It allows you to execute calls on transfers and approvals both before and after tokens are transferred, regardless of whether the receiving address is a contract or not. 

## Standards for multiple token
* **ERC-1178:** The ERC1178 contract allows for multiple types of collectibles to be defined, which means that any number of a given type of collectible can be transferred at once. This is particularly useful for less expensive collectibles that might not have much value individually but could be quite valuable when bought in bulk.

## Some other Standards 
* **ERC-981: **The purpose of this proposal is to introduce a new Ethereum Interface that would allow asset owners to issue tokens in a marketplace. This would be done by dividing the asset into divisible units, which in turn would increase the fungibility of that asset. Doing this would create more opportunities for those who own a finite quantity of an asset to trade it.

    


---
## Evaluation





##### What feature of ERC-1404 gives more control to the creator as compared to ERC-20?  
     
- [ ]  to prevent unintentional token sends to contracts
- [x]  greater control over token circulation
- [ ]  to specify the total supply of tokens
- [ ]  to specify the owner of the token





##### How does ERC-1190 help creators?  
     
- [ ]  Allows for the creation of unique digital assets that cannot be replicated
- [x]  Creators can earn benefits every time rights of thier object is used
- [ ]  Aims to provide a way to register land and physical property on the Ethereum blockchain
- [ ]  It helps to rent NFTs





##### How are tokens transferred via ERC-965?  
     
- [ ]  via on chain transaction
- [ ]  by calling sendByCheque() method
- [ ]  sending the tokens to a third party
- [x]  both A and B

    

