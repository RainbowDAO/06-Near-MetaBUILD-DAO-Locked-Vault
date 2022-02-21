![](https://raw.githubusercontent.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/main/pic/Banner.png)
# Submission for the NEAR MetaBUILD Hackathon



# DAO Locked Vault System



#  Project submission information


## 1.Project name

DAO Locked Vault System 

## 2.Elevator pitch

Through our DAO lock-up vault system, a certain amount of ERC20 tokens can be locked according to the specified rules and released according to the corresponding rules.

## 3.Team Name

RainbowCity Foundation



## 4.Submission links

In this NEAR MetaBUILD Hackathon event, RainbowCity Foundation submitted a total of 10 projects, which is the  address directory of the 10 projects. We are continuing to refine the details of each project.

- Submission address directory:
- https://www.rainbowdao.io/NearMetaBUILD



- Project demo website:
- https://lockedvaultnear.rainbowdao.io/
- GitHub repository :
- https://github.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault
- Solidity-Version-contract (GitHub): 
- https://github.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/tree/main/Solidity-version-contract-for-Aurora
- Frontend code (GitHub):
- https://github.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/tree/main/Front-end-for-Solidity-version
- Picture (GitHub): 
- https://github.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/tree/main/pic


## 5.Recorded video demo


https://youtu.be/YZBzZuV1src



## 6.Testnet Deployment Information


- Aurora testnet address: 

https://testnet.aurora.dev/


- Contract deployment address

vault:0x0b0220C342536171495057c6bC7421e9dA2D6f02



RBD:0x8408d82B9A7FB70F314A85ba444b0e0ECeCe482E



Frontend docs:

https://github.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/blob/main/Front-end-for-Solidity-version/README.md

Contract  docs: 

https://github.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/blob/main/Solidity-version-contract-for-Aurora/README.md



## 7.What is the RainbowCity Foundation？

Headquartered in Singapore, RainbowCity Foundation is a non-profit foundation founded by Mr. Kunyuan, which mainly engages in the incubation and investment of the crypto ecosystem. Being a big fan of Bitcoin, Mr. Kunyuan worships Satoshi Nakamoto and dedicates himself to the spread of Satoshi Nakamoto’s great ideas of decentralization. He once put forward the concept of “Bit Civilization” for the first time in the world in July 2021 at the Bitcointalk Forum established by Satoshi Nakamoto. Moreover, he wrote over 50 articles to promote Bitcoin, in the hope of fostering the development of the encryption industry worldwide and practicing the true Bitcoin spirit.

Mr. Kunyuan has had rich experiences in the crypto world. At one time, he was the highest community leader of FCoin, the most influential community exchange in the Chinese world. In November 2018, in a referendum on the FCoin exchange, Mr. Kunyuan was elected the first community committee member and then appointed vice Chairman to fully preside over the work of the FCoin community.

Mr. Kunyuan believes that a super economic powerhouse will emerge in the mankind history in the future; a crypto world which is constructed in the form of decentralized protocols that transform all different decentralized behaviors into a unified economy. He believes it will ultimately become the infrastructure of human civilization and this is in which the RainbowCity foundation originates from this belief.

The RainbowCity Foundation aims to invest in seven major industries in the following ten years, including Rainbow DeFi, Rainbow Investment, Rainbow Culture, Rainbow Network, Rainbow Industry, Rainbow Education and Rainbow R&D. It strives to become a super economic hub with market value worth one trillion US dollars.


## 8.Project social media: 

RainbowDAO website ：http://www.rainbowdao.io

Rainbowcity website ：https://www.rainbowcity.io

Twitter:    https://twitter.com/RainbowDAOio

Discord     https://discord.gg/vbnvFEeYRr   

Telegram: https://t.me/RainbowDAO

Medium:   https://medium.com/rainbowcity

Github:    https://github.com/RainbowDAO

Email： Rainbowcitydao@gmail.com





#  Project Story

## 1.Inspiration



The DAO lock-up vault system is also a very practical Web3 tool developed by us, especially suitable for various types of DAO governance. Each DAO organization will issue its own governance tokens, and will also manage its own governance tokens. Locking is a very common application scenario, but there is no corresponding tool in the market. What we solve is the basic need of ERC20 token lock-up.

## 2.What it does



Through our DAO lock-up vault system, a certain amount of ERC20 tokens can be locked according to the specified rules and released according to the corresponding rules.

It is mainly suitable for two important application scenarios. The first point is to issue private tokens to early investors of a project. Tokens issued by early investors need to follow certain rules for lock-up, and the corresponding tokens can only be released after the lock-up time expires.

The second point is the token incentives that can be used for community members or core employees of the DAO organization. In order to reward core community members and core employees, some governance tokens will be issued for incentives, but the issued governance tokens are not immediately available for circulation, but need to follow certain lock-up rules. In this way, the interests of core members can be aligned with the interests of the DAO organization.


## 3.How we built it

![image](https://raw.githubusercontent.com/RainbowDAO/01-Near-MetaBUILD-RainbowDAO-Factory/main/pic/Logic-diagram/06-Logic-diagram-of-lock-vault.png)

Operation steps of the DAO lock-up vault system function:

### ⑴ Create a lock-up vault and initialize the vault

First, you need to initialize the name, profile, logo, and basic information of the lock-up vault. Then set the time of the complete closure period. The complete closure period refers to the period in which the governance tokens are completely locked without any release after they are locked.

Set the starting release time, the monthly release proportion after the starting release, and the final time when the vault is fully unlocked.

For example, the complete closure period is 24 months, which is equivalent to that no one can withdraw money from the lock vault within 24 months; If the release rate is 2% per month during the release period, it will take 50 months for 100% to be released. The final full unlocking period is 24 + 50 = 74 months.



### (2) deposit in the lock vault

To make a deposit to a locked bank, you need to specify the recipient's address. There are two situations:

① Drawn by the depositor;

② Authorized by the depositor to receive, authorized to receive can authorize multiple addresses to receive, and each address can receive a corresponding share of tokens according to the proportion;

### ⑶ Whether the depositor can terminate the authorization to collect, there can be two different application scenarios:

① In the first case, when the tokens are sold privately, the project party can deposit the corresponding tokens into the lock vault and authorize the private buyer to receive them at the agreed time. At this time, the project party does not need to have the authority to terminate the authorization. When the project party deposits the token into the lock vault, it will no longer have the management authority of this fund.

② The second case is employee incentives. The project party and employees agree on a certain number of token incentives, and employees can receive corresponding rewards after completing corresponding tasks. During this process, if the motivated employee resigns or fails to complete the corresponding assessment, the depositor can cancel the corresponding reward. At this time, the depositor needs to terminate the authorization to receive and cancel the corresponding reward.

If there are multiple recipient addresses authorized, the depositor can choose to terminate one or more of them, or terminate all of them, and the corresponding withdrawal authority will be changed back to the depositor itself.



### ⑷ Lock-up bank withdrawal

The depositor or the authorized receiving address will receive the corresponding funds from the lock-up vault according to the lock-up agreement.


## 4.Challenges we ran into

Combing the logic of the product remains our biggest challenge in developing this lock-up vault. We must consider the application scenarios of various types of DAO organizations issuing governance tokens for lock-up, and combine the actual scenarios to develop products that meet market needs. Only in this way can our products be truly applied to the actual DAO governance.

## 5.Accomplishments that we're proud of

Our greatest achievement in this product development is that we not only solved the problem of private placement locking, but also developed a locking scheme for employee incentive payment, and combined these two different needs to build a very complete and practical product.


## 6.What we learned

Through this product development, we have a deeper understanding of the different needs of various DAO organizations in the management and issuance process of governance tokens, which allows us to have a deeper understanding of the governance needs of DAOs, which will help Because we develop products that can truly meet the actual needs of the industry.

## 7.What's next for DAO-Multi-Signature-Committee 

Our next main work is to continue to sort out the details of this product, reconstruct the logic of the product, and make this product as adaptable as possible to the needs of various types of DAO organizations. When the product functions are further improved, we will submit an external audit, and when the audit is completed, we will deploy the product to each public chain.



#  Project UI



##  1-Locked-Vault-System-1



![image](https://raw.githubusercontent.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/main/pic/1-Locked-Vault-System-1.png)



##  2-Locked-Vault-System-2



![image](https://raw.githubusercontent.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/main/pic/2-Locked-Vault-System-2.png)



##  3-Locked-Vault-System-3



![image](https://raw.githubusercontent.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/main/pic/3-Locked-Vault-System-3.png)




##  4-Deposit



![image](https://raw.githubusercontent.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/main/pic/4-Deposit.png)



##  5-Home




![image](https://raw.githubusercontent.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/main/pic/5-Home.png)



##  6-Info



![image](https://raw.githubusercontent.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/main/pic/6-Info.png)




##  7-Info-Withdraw



![image](https://raw.githubusercontent.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/main/pic/7-Info-Withdraw.png)




##  8-Manager



![image](https://raw.githubusercontent.com/RainbowDAO/06-Near-MetaBUILD-DAO-Locked-Vault/main/pic/8-Manager.png)

