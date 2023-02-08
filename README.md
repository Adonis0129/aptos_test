Simple Forum Page

This website allows users to post, reply, like, and unlike.

Link: https://aptos-test-mu.vercel.app

How to start
- npm install
- npm start


This project involves front-end development, back-end (smart contract) development, and web3 integration. 
The front-end was developed in React with TypeScript and Material UI.
I created the smart contract for the back-end, and all data is stored in the smart contract.
The smart contract was written in the Move language and deployed on the Aptos test network. 
To create the smart contract, I used the vector and resource account concepts of the Move language, and the data is stored in the form of arrays on the Move chain. 
This project can be tested using wallets that support the Aptos network, such as Pontem, Petra, and Martin, among others.

Whenever the wallet, post, vote, or reply is changed, all data is loaded again from the smart contract. This allows users to see all updates as soon as they vote, post, or reply. When a post, reply, or vote is made, the front-end calls the corresponding function in the smart contract, which adds and sorts the data on the Move chain. For example, when the post button is clicked, the front-end calls the post function in the smart contract, and the post data is stored on the Move chain.
The poster can not reply or vote regarding to their posted data.

The challenge was to find the correct position in the array when users voted and replyed. To solve this issue, I used the index concept in the smart contract. When the data is received from the smart contract, I had to sort it again so that it could be used in the dapp. 
I have thoroughly tested all functionalities, and everything is working as expected.