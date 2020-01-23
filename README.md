## VGS Collect iOS SDK Demo

This examples shows how easily you can integrate <a href="https://github.com/verygoodsecurity/vgs-collect-android">VGS Collect iOS SDK</a> 
into your application and secure sensitive data with us.

<p align="center">
    <img src="./vgs-collect-ios-demo-gif-low.gif" width="250">
</p>

## How to run it?

### Requirements

- Installed <a href="https://apps.apple.com/us/app/xcode/id497799835?mt=12" target="_blank">Xcode</a>
- Installed <a href="https://guides.cocoapods.org/using/getting-started.html#installation" target="_blank">CocoaPods</a>
- Organization with <a href="https://www.verygoodsecurity.com/">VGS</a>


#### Step 1

Go to your <a href="https://dashboard.verygoodsecurity.com/" target="_blank">VGS organization</a> and establish <a href="https://www.verygoodsecurity.com/docs/getting-started/quick-integration#securing-inbound-connection" target="_blank">Inbound connection</a>. 

#### Step 2

Clone demo application repository.

``git clone git@github.com:verygoodsecurity/ios-sdk-demo.git``

#### Step 3

Install demoapp pods.

Open Terminal and change working directory to `demoapp` that is inside `ios-sdk-demo` folder:

`$ cd ~/demoapp`

Install pods:

`pod install`


#### Step 4

In `demoapp` folder find and open `demoapp.xcworkspace` file.
In the app go to `ViewController.swift` file, find the line

`var vgsForm = VGSCollect(id: "VaultId", environment: .sandbox)`

and replace `VaultId` with your organization
 <a href="https://www.verygoodsecurity.com/docs/terminology/nomenclature#vault" target="_blank">vault id</a>. 
 
### Step 5 

Run the application and submit the form. 
Then go to the Logs tab on <a href="http://dashboard.verygoodsecurity.com" target="_blank">Dashboard</a>, find request and secure a payload. 
Instruction for this step you can find <a href="https://www.verygoodsecurity.com/docs/getting-started/quick-integration#securing-inbound-connection" target="_blank">here</a>.

### Useful links

- <a href="https://www.verygoodsecurity.com/docs/vgs-collect/ios-sdk" target="_blank">Documentation</a> 
- <a href="https://github.com/verygoodsecurity/vgs-collect-ios" target="_blank">Repo</a> 
- <a href="http://cocoapods.org/pods/VGSCollectSDK" target="_blank">CocoaPods</a> 


