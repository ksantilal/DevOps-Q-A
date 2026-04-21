Deployment Stratagies
-----------------------------
* What is Deployment?
    - Desire State 

    
* What is deployment stratagies


- 1. Recreate
    - Your pod will be stop and delete and recreate so you will have downtime that is why it is not use for production.

- 2. Rolling Update
    - Your pod will be update one by one so you will not have downtime and it is use for production.

- 3. Blue/Green
    - You will have two environment one is blue and another is green and you will deploy your new version in green environment and after that you will switch the traffic to green environment and blue environment will be idle and you can delete it later.

- 4. Canary
    - You will deploy your new version in a small percentage of your pods and after that you will monitor the performance and if everything is fine then you will deploy it to all pods.
