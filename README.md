
# ScreenShots

<p align="center">
  <img src="https://github.com/ikeuzo57/AndroidPaypal/blob/master/ScreenShots/pic1.jpeg" width="200"/>
  <img src="https://github.com/ikeuzo57/AndroidPaypal/blob/master/ScreenShots/pic2.jpeg" width="200"/>
  <img src="https://github.com/ikeuzo57/AndroidPaypal/blob/master/ScreenShots/pic3.jpeg" width="200"/>
  <img src="https://github.com/ikeuzo57/AndroidPaypal/blob/master/ScreenShots/pic4.jpeg" width="200"/>
</p>


# PayPal Android Example
Mini E-commerce android application that uses PayPal gateway with Node.js backend to verify payments and Firebase as database to store
products , sales and payment information .

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

* <a href="https://git-scm.com/">git</a> 
* <a href="https://www.npmjs.com/package/npm">npm install</a>  
* <a href="https://nodejs.org/en/download/">node.js</a> 
* facebook app to get facebook_app_id .
* firebase account . 
* PayPal Account .
* <a href="https://dashboard.heroku.com/">Heroku</a> account if u want to deploy live . 


### Installing

* clone the project then navigate to server folder and execute 

```
npm install
```
  this command will install the required libraries that will be used for our Node.js back-end .


* assuming you already created firebase project :- <br/>
  + Import ***database.json*** file in project folder to your firebase project database.
  + Enable Facebook Authentication from firebase project dashboard . 
  + Generate New Private Key : <br/> 
    Project Setting -> SERVICE ACCOUNTS -> Firebase Admin SDK -> GENERATE NEW PRIVATE KEY <br/>
    this will create and download .json file containing the required credentials for firebase admin . <br/>
  + ***Copy*** the downloaded file into ***node_modules*** folder.

* go to <a href="https://developer.paypal.com/developer/applications/">PayPal developer</a> :- <br/>
  + create new App to get the  ***client_id*** and ***client_secret*** <br/>
  + create two accounts ( Business - Personal ) to be used for testing .
  
* open ***index.js*** file and do the necessary changes . 


### Running the tests

* first step is to run our server locally so navigate to server folder and execute 
```
node index.js
```
<space><space><space>if everything works as expected you should see a log messages says 
```
Magic happens on port 5000
```
* open Android Studio and import the Android project then go to ***strings.xml*** and ***Config.java*** file and do the nessecary changes .
* add google-services.json file of your firebase project to the android app folder . 

* when you come to the part where u should enter paypal login info to complete the buying process , login with the personl account     previously created for testing then login to <a href="https://www.sandbox.paypal.com/">paypal sandbox</a> with the Business account to see the transactions .<br/>
  
* That's it you did it :) <br/>

#### Dependencies

* Android-ActionItemBadge - https://github.com/mikepenz/Android-ActionItemBadge  <br/>

#### Developed By 
* Ike
* ikeuzo57@gmail.com
* <a href="https://www.paypal.me/Ikechukwu">paypal.me/Ike</a> <br/>

#### License
```
Copyright 2017 Ikechukwu

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.

```
