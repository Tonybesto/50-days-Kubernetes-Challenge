

## Image Build Info

| Item      | Description |   
| :---        |    :----:   |  
| Base  | node:8.9-alpine |  
| Work Directory  |  /app |     
| Build Instructions  |  Refere Below |  
| Ports | 80 |  
| Launch Command | node server.js |  

### Build Instrcutions

```
npm install -g nodemon
npm config set registry https://registry.npmjs.org

npm install \
 && npm ls \
 && npm cache clean --force \
 && mv /app/node_modules /node_modules
```
