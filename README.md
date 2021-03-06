# WebdriverIOTypeScriptBDD
This is a sample Cucumber Framework that uses WebdriverIO and TypeScript. This project is useful not only as an example of WebdriverIO and TypeScript playing nicely together, but it also includes some practical examples of the Page Object design pattern


### Requirements
-   node >= 12.18.x - [how to install Node](https://nodejs.org/en/download/)
-   npm >= 6.14.x - [how to install NPM](https://www.npmjs.com/get-npm)

### Getting Started
Clone Repository
```bash
1. git clone https://github.com/sadabnepal/WebdriverIOTypeScriptBDD.git
2. Navigate to `WebdriverIOTypeScriptBDD`
```

Install the dependencies:
```bash
npm install
```

Run e2e tests:
```bash
npm test
```

Generate allure report:
```bash
npm run report
```

### Folder Structure
```
├───drivers
|       ├───chromedriver_win32.zip
|       └───geckodriver.exe
├───src
|   ├───constants
|   │       └───accounts.ts
│   ├───enums
|   │       └───WaitEnums.ts
|   ├───features
|   │       └───TC01_CreateAccount.feature
|   │      
|   ├───pages
|   │  	    ├───AuthenticationPahe.ts
|   │	    ├───BasePage.ts
|   │	    ├───CreateAccountPage.ts
|   │	    └───HomePage.ts
|   ├───stepdef
|   │       └───TC01_CreateAccount.spec.feature
|   │      
|   └───testdata
|           └───SignUp.json
├───Utils
|       ├───Utilities.ts
|       ├───AssertionUtils.ts
|       └───WaitUtils.ts
├───package.json
├───README.md
├───tsconfig.json
└───wdio.conf.ts
```

### Runing a Test in firefox
```bash
---------------------------------------------------------------------------------------------------------
Use only if `selenium-standalone` does not work inside proxy network
---------------------------------------------------------------------------------------------------------
1. Uncomment `firefox configuration` from `capabilities section` present in `wdio.conf.js` file
2. Run below command `npm run startFirefox` in terminal and leave it open 
	**Note: Make sure you enter correct path of firefox installed in your system in package.json file
3. Open new terminal and run `npm test`. Execution will start in both chrome and firefox
```

### Inside Corporate network If fails to download driver files then:
```bash
Download the latest driver from `https://chromedriver.chromium.org/downloads`
Delete the existing `chromedriver_win32.zip` file and add newly downloaded zip file 
Run `installchromedriver.bat` command from cmd or double click on bat file
It will download the driver from `drivers-->chromedriver_win32.zip`

```

### Sample Report
![image](https://user-images.githubusercontent.com/65847528/119223707-8a5ea600-bb18-11eb-8d49-1b845814bcb8.png)

