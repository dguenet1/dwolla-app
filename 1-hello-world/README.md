# Hello World

1. Download [Node.js](https://nodejs.org/en/)
2. Create your application

```
mkdir myapp
cd myapp
npm init
```

3. Install Express.js

```
npm install express --save
```

4. Create app.js file in root of project and add the following code

```javascript
const express = require("express");
const app = express();
const port = 3000;

app.get("/", (req, res) => res.send("Hello World!"));

app.listen(port, () =>
  console.log(`Dwolla App listening at http://localhost:${port}`)
);
```

5. In package.json in the root change the main to `"main": "app.js",`
6. From the root of the project in your terminal run the following code

```
node app.js
```

## Resources

- https://nodejs.org/en/
- https://expressjs.com/en/starter/installing.html
- https://expressjs.com/en/starter/hello-world.html
