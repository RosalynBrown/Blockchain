
# Blockchain

1. First I navigated to the Blockchain folder where my Ethereum Tools are saved then created my first node named “one” using the code below. I noted the public address to use later.

`./geth --datadir one account new`

Public address of the key:   0x2A1B6153666d0b657fffb13Ed576728f730Bac4C
Path of the secret key file: one/keystore/UTC--2021-08-27T23-21-05.519760000Z--2a1b6153666d0b657fffb13ed576728f730bac4c

<img width="294" alt="Picture1" src="https://user-images.githubusercontent.com/82069175/131203632-cea7eb27-dd96-4127-a58f-99611f757894.png">

2. 2.	Next I set up my next node using the code below with the name “two” and making note of the public key to use later. 

` ./geth --datadir two account new`

Public address of the key:   0x5e4ED64B80314020c971B1D168D81c3bC30824Ef
Path of the secret key file: two/keystore/UTC--2021-08-27T23-22-01.678087000Z--5e4ed64b80314020c971b1d168d81c3bc30824ef

<img width="292" alt="Picture2" src="https://user-images.githubusercontent.com/82069175/131227710-92cf81e2-b82a-4bcf-9d63-e31741ea8a88.png">

3. 3.	Next initiate puppet with the command below

`./puppeth!`

4. 4.	Next I created the network name “three”. I went through the prompts to configure and create a new genesis from scratch. Based on the instructions I used selected proof of assignment for this activity. With just 2 nodes I selected a short time period of just 4 seconds. 

<img width="383" alt="Picture3" src="https://user-images.githubusercontent.com/82069175/131227774-6e6fbfe9-1c18-4acb-a7b9-08bf815d1e1a.png">

5. 1.	Next I attached the public address for my 2 nodes “one” and “two” in order to seal them. They were also the accounts selected to be prefunded. Per the instructions I did not prefund with 1 wei. I selected the network ID to be 777. Following that I exported the genesis configurations so I could use the three.json later.

<img width="468" alt="Picture4" src="https://user-images.githubusercontent.com/82069175/131227794-fe73cb0f-7e87-4668-86ec-c209212bd730.png">

6. 6.	At this time I iniitated the nodes by opening 2 bash terminals and running the following commands 1 in each window.

`./geth --datadir one init three.json`

<img width="468" alt="Picture5" src="https://user-images.githubusercontent.com/82069175/131228549-e55145d6-7e4b-4d66-9897-bcc66665e09c.png">


7. 7.	This command was run in the second window![image](https://user-images.githubusercontent.com/82069175/131228559-944a23ba-d71a-49fe-a728-0aae83bf7a05.png)















