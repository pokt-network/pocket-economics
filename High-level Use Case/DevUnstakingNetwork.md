# High-Level Use Case / Developer Unstaking in/from the Network

### Use Case Description
This high-level use case describes a developer unstaking some amount of POKT after the bonding period and during the bonding period. It will also describe a developer unstaking all of their POKT which removes them from being an active actor in the network. <br/>

See below for questions and answers.

### Pre-Conditions
The developer is an active user in the Pocket Network and has some amount of POKT staked.

### Post-Conditions
1. The developer is still an active user in the Pocket Network but has unstaked some amount of their POKT.

2. The developer is no longer an active member in the Pocket network and has unstaked all of their POKT.

### Actors
Developer, Developer Portal, System

### User Story
I am a developer in the Pocket Network. I have been **staked for a minimum of 3 eras** (approx. 3 weeks) and I would like to unstake some amount of the POKT I have staked in the network.

1. Developer visits the developer portal.
2. Developer logs into their account.
3. System confirms.
4. Developer enters in the amount of POKT they wish to unstake.
5. System confirms.
6. System sends returned POKT amount to developers wallet.

I am a developer in the Pocket Network. I have been **staked for less than 3 eras** and I would like to unstake some amount of the POKT I have staked in the network.

1. Developer visits the developer portal.
2. Developer logs into their account.
3. System confirms.
4. Developer enters in the amount of POKT they wish to unstake.
5. System sends error **User is still bonded**.
6. Developer confirms amount to unstake
7. System confirms.
8. System calculates amount of POKT to burn and amount of POKT to return.
9. System burns (appropriate amount) of POKT.
10. System sends balance of returned POKT to developers wallet.

I am a developer in the Pocket Network. I have been staked for a minimum of 3 eras (approx. 3 weeks) and I would like to unstake all of the POKT I have staked in the network resulting in my exit of the network.

1. Developer visits the developer portal.
2. Developer logs into their account.
3. System confirms.
4. Developer enters in the total amount of POKT staked.
5. System sends error **Confirm you are about to leave the network.**
6. System sends total POKT amount to developers wallet.

### Questions
1.  How often can I unstake? <br/>
	A) A developer can enter in the amount of POKT they wish to unstake anytime but the system will only release the POKT to them at the end of the era.
2. Do I need to wait until the end of the third era before I unstake? <br/>
	A) No, a developer can unstake before the end of the third era but there will be a penalty for unstaking early (before the bonding period is over). <br/>
3. What is the penalty for unstaking before the bonding period is over? <br/>
	A) In the case of unstaking during the bonding period, a portion of the stake is burned while a portion is returned; the amount returned is directly proportional to how long the stake has been in the network.
4. If I am at the end of my bonding period and I stake more POKT to increase the number of relays I am receiving, what happens to the bonding period? <br/>
	A) 	When a developer stakes POKT the bonding period resets. 
	