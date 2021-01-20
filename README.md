# UPSTAC APPLICATION

### API Requirements and Goals
- Implement and update the Lab Request and Consultation Feature in the UPSTAC API application in UPSTAC backend . 

- With respect to the Tester, complete the code in 'LabRequestController' class  to view the open test requests, assign the tests to themselves and finally update the test results.
- With respect to the Doctor, complete the code in ‘ConsultationController’ class to view the pending test results, assign consultations to themselves and update the doctor suggestions.


#### UPSTAC Backend
To run backend code, Run ‘UpstacApplication.java’ file.


#### UPSTAC-UI 

$ cd upstac-ui
$ npm install -g yarn
$ yarn install
$ yarn clean cache
$ yarn start


#### MYSQL

$ docker network create dev-network-upstac
$ docker run --restart always --name mysql8.0 --net dev-network-upstac -v /Desktop/UPSTAC/UPSTAC/mysql/mysql_data/8.0:/var/lib/mysql -p 3306:3306 -d -e MYSQL_ROOT_PASSWORD=password mysql:8.0


--------------------------------
Note: To manual authorisation of the tester on DataBase please update status to 1

UPDATE `upgradpg`.`user` SET `status` = '1' WHERE (`id` = '8');

