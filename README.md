# ServeRest

#### Prerequisites
- Have node.js installed on the machine
- Have newman installed on the machine, just run the command in node.js cmd:
```sh
npm install -g newman
```
- Download the project to the machine in directory "C:"

#### Run project
1. Run the project open node.js cmd
2. Change directory to ./ServeRest
3. Run the newman command:
```sh
newman run ./postman/collections/Users/.resources/Users.postman_collection.json -e ./postman/collections/Users/.resources/enviromentServeRest.postman_environment.json --reporters cli,json --reporter-json-export ./postman/reports/reportsServeRest.html

#### View BDDS
Access the following path:
Create User: ./postman/collections/Users/Create User/.resources/definition.yaml
Get User: ./postman/collections/Users/Get User/.resources/definition.yaml
Update User: ./postman/collections/Users/Update User/.resources/definition.yaml
Delete User: ./postman/collections/Users/Delete User/.resources/definition.yaml

#### View logs
Access the following path ./postman/reports/reportsServeRest.html