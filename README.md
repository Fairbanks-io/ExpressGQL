# ExpressGQL

Express GraphQL Server with Lusca and DDoS Rate Limiting

#### Prerequisites
- Node v8+
- Yarn (prefered) or NPM
- Port 8888 Open and Accessible

#### Quick Start
- Fetch the code using git or wget
- While in the app directory, `yarn` or `npm install` to setup
- Once complete, `yarn start` or `npm start` to launch the server
- Navigate to <host>:8888 in your browser

*[Optional] To keep ExpressGQL up and running behind the scenes, checkout [PM2](http://pm2.keymetrics.io/ "PM2").*


#### Config Options
The following options can be passed in at runtime as ENV variables:
- `SESSION_SECRET`: Either a string or array of secrets used to sign the session ID cookie (If array: first is used to sign, others are used to verify)
- `LOGGING`: If **true**, a graphql.log will be created for incoming site requests using Morgan logging
- `RATE_LIMIT`: If **true**, enables DDoS and RateLimit protections through Express
- `PORT`: If set, an alternate port will be used when starting ExpressHTTP. Otherwise, the default of **8888** will be used.