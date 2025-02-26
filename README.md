# Getting Started

Welcome to your new project.

It contains these folders and files, following our recommended project layout:

File or Folder | Purpose
---------|----------
`app/` | content for UI frontends goes here
`db/` | your domain models and data go here
`srv/` | your service models and code go here
`package.json` | project metadata and configuration
`readme.md` | this getting started guide


## Next Steps

- Open a new terminal and run `cds watch` 
- (in VS Code simply choose _**Terminal** > Run Task > cds watch_)
- Start adding content, for example, a [db/schema.cds](db/schema.cds).


## Learn More

Learn more at https://cap.cloud.sap/docs/get-started/.


## Create a Business Service with Node.js Using Visual Studio Code 

npm i -g @sap/cds-dk

cds

cds init bookshop

cd bookshop

cds add samples

code .

npm install

Package.json kind: sql

npm i sqlite3 -D  

cds deploy --to sqlite:db/my-bookshop.db

sqlite3 db/my-bookshop.db -cmd .dump  (Check .tables, Exit .quit)

cds watch

Test Postman  (Import File Postman.json in the wizard)

Package.json kind: Hana

npm add @sap/hana-client --save

cf create-service hanatrial hdi-shared my-bookshop-db

cds build --production   (create tables and manifest.yaml)

cf push -f gen/db

cf push -f gen/srv --random-route  (create app)

cf apps

-Update-

cf delete myapp (optional)

cf push

cf logs myapp --recent

cf logs myapp | findstr /V RTR
