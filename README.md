ng new remote
ng add @nguniversal/express-engine
npm run dev:ssr
ng add @angular-architects/module-federation@15 --project remote
ng build --watch
ng run remote:server
npm install cors
node dist/remote/server/main.js
