# KafkaMiniProject
Simulated streaming fraud detection app

## Steps to replicate the project
1. Prerequisits: must have docker installed and running
2. Clone/download the repository
3. Navigate to the repo directory in terminal
4. Run docker-compose -f docker-compose.kafka.yml up
5. Open a new terminal tab and run docker-compose up
6. Open a third tab and run 'docker-compose -f docker-compose.kafka.yml exec broker kafka-console-consumer
--bootstrap-server localhost:9092 --topic streaming.transactions.legit' to test if the legit branch is produced correctly
7. Open a fourth tab and run 'docker-compose -f docker-compose.kafka.yml exec broker kafka-console-consumer
--bootstrap-server localhost:9092 --topic streaming.transactions.fraud' to test if the fraudelent branch is produced correctly

![Screen Shot 2022-05-25 at 7 23 21 PM](https://user-images.githubusercontent.com/20688436/170402550-4ffba876-a408-4923-be93-65e016567142.png)

<img width="705" alt="Screen Shot 2022-05-25 at 7 26 49 PM" src="https://user-images.githubusercontent.com/20688436/170403272-fc973aaa-8792-43f4-be1d-8cf17ef0b570.png">

<img width="655" alt="Screen Shot 2022-05-25 at 7 29 13 PM" src="https://user-images.githubusercontent.com/20688436/170403281-b47925c1-29be-4c94-98b4-afccd6d9420c.png">
