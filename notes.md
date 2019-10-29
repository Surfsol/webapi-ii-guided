1. npm init -y  (creates package.json)



to run a script, named test: npm test

if install as a deve dependence -D, will only be used in development, will not be pushed to production.  will show in deve dependentcies
npm i nodemon -D 

2. can bring up to
 scripts 
'dev' = 'nodemon'

3. "main" = 'main.js'

main is first file to execute, normally index.js

4. npm i nodemon -D

to install globally
npm i -g nodemon

5. npm run dev 
- will run main.js

6. npx gitignore node

7. in main.js
const express = require('express')

const server = express()

server.get('/', (req, res) => {
    res.json({api: 'running'})
})

const port = 8888
server.listen(port, () => console.log('server running'))

8. npm run dev


Can break APIs into Routers

/api/hubs
/api/users
/api/messages
/api/lessons

REST.
-everything is a Resource
-Resources are accessed through a single URL