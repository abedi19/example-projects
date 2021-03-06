A trivial Node.js microservice example, that just returns a different superlative message each time, as a demonstration of using external NPM modules packaged with the Lambda function. (In this case, the superlatives come from the [Superb](https://www.npmjs.com/package/superb) NPM module. 

To try it out, first [set up the credentials](https://github.com/claudiajs/claudia/blob/master/getting_started.md#configuring-access-credentials), then:

1. run `npm install` to grab the dependencies
2. run `npm start` to set up the lambda project under the default name on AWS 
3. run `npm test` to execute the lambda from the command line and print the output on the console

Re-run the test again to see a different message. Check out the [package.json](package.json) scripts section to see how Claudia gets invoked for the `start` and `test` scripts. Check out the [main.js](main.js) file to see how the Lambda function works. For a bit more fun, modify the code in [main.js](main.js), then run `npm run deploy` to deploy the code to AWS, then run the test again to see the change.
