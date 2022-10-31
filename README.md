# Quick Guide To Run SIDE Tests On a Cloud Selenium Grid
# Prerequisites

The first step is to download and install Node.js and node package manager or npm. We recommend using the latest version of node.js.

You can download it from official [NodeJS website](https://nodejs.org/en/).

If you have npm already installed, you may want to upgrade it to the latest version. Here the code you can run in your terminal to upgrade npm.

```
npm install npm@latest -g
```


After Node.js and npm is installed we need to install the dependencies. Run below code to install the required packages. 

```
npm install -g
```

# Executing The Test On LambdaTest
Please update the capabilities file *side.yml with your test requirements and update the server username and access key which you can find on lambdatest dashboard. 

Note: You can generate capabilities for your test requirements with the help of our inbuilt [Capabilities Generator tool](https://www.lambdatest.com/capabilities-generator/).

```
capabilities:  
  LT:Options:
    browserName: Firefox    
  browserName: Firefox
  version: 103
  platform: Windows 8
server: "https://username:accesskey@hub.lambdatest.com/wd/hub"
```

Once the capabilities are set. Please execute the following command below to run your tests

```
npm test
```

### Now Head over to the Lambdatest Automation Dashboard where you can see your test results.

# Additional Links
[How To Run Selenium IDE Test Over Online Selenium Grid?](https://www.lambdatest.com/blog/run-selenium-ide-test-on-online-selenium-grid/)
