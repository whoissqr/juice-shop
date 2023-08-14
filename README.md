# seeker instrumentation

## method 1:
```
git clone https://github.com/juice-shop/juice-shop
cd juice-shop
npm install --strict-ssl=false --prefix seeker "https://testing.seeker.synopsys.com/rest/api/latest/installers/agents/binaries/NODEJS?projectKey=juiceshop-shichao&flavor=TARGZ"
npm install

export SEEKER_SERVER_URL=https://testing.seeker.synopsys.com:443
export SEEKER_PROJECT_KEY=juiceshop-shichao
export NODE_OPTIONS="-r ./seeker/node_modules/@synopsys-sig/seeker"
npm start
curl http://localhost:3000
```

## method 2:
npm install --strict-ssl=false --prefix seeker "https://xxx.seeker.synopsys.com/rest/api/latest/installers/agents/binaries/NODEJS?projectKey=juiceshop-shichao&flavor=TARGZ"

npm start
curl http://localhost:3000
