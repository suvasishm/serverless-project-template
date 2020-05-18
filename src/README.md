This is a template for a serverless function/application and local test.

#### Execute the following to create a new function and its test
```$ serverless create function -f <function_name> --handler src/functions/<function_name>.<function_name> --path src/tests```

Note: Replace <function_name> with actual function name. This will do the following:
- create src/funtions/<function_name>.js
- create src/tests/<function_name>.js
- update serverless.yml and add the function handler under functions.

#### Test the newly created function using the mocha plugin
$ mocha src/tests

Start building your serverless appliction from here!


### Prerequisites:

Execute the following commands to ready your local environment before doint the above.

#### Install the following serverless plugins
```$ serverless plugin install --name serverless-pseudo-parameters```

```$ serverless plugin install --name serverless-mocha```

Note: The above would add a plugins section in the serverless.yml

#### Install the following plugins
```$ npm install --save-dev aws-sdk-mock```

```$ npm install --save-dev mocha```
