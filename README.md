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


## Create a Business Service with Node.js Using Visual Studio Code (Commands)

npm i -g @sap/cds-dk
cds

cds init bookshop
cds add samples

code .

npm install
cds watch

npm i sqlite3 -D

cds deploy --to sqlite:db/my-bookshop.db

sqlite3 db/my-bookshop.db -cmd .dump

npm add @sap/hana-client --save

cf create-service hanatrial hdi-shared my-bookshop-db

cds build --production   (create tables and manifest.yaml)
cf push -f gen/db
cf push -f gen/srv --random-route

name:              my-bookshop-srv
requested state:   started
routes:            my-bookshop-srv-....cfapps.....hana.ondemand.com

-Update-

cf delete myapp
cf apps

cf push

cf logs myapp --recent

cf logs myapp | findstr /V RTR
