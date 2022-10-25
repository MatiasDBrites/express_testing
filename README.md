# express_testing

Despues de hacer migraciones

se instala 

npm i cross-env

npm i mocha   

npm i chai     

npm i supertest

agregar packed.jsom

 "scripts": {
    "start": "nodemon app.js",
    "test": "cross-env ENV=test mocha ./__test__/*",
    "pretest": "cross-env NODE_ENV=test npm run db:reset",
    "db:reset": "npx sequelize-cli db:drop && npx sequelize-cli db:create && npx sequelize-cli db:migrate",
    "db:create:test": "cross-env NODE_ENV=test npx sequelize-cli db:create"
  },
  
  agregar mocha.opts
  
  --file ./__tests__/teardown.js
  
  crear carpeta /__test__
  
  crear archivo test.auth.js
  
  crear archivo teardown.js
  
  modificar ./config/config.json
