# DreamHouse Mobile App

## Install the Application

1. Install the latest version of Cordova and Ionic 2 beta:
    ```
    npm install -g cordova ionic@beta
    ```

    or

    ```
    sudo npm install -g cordova ionic@beta
    ```

1. Clone this repository
    ```
    git clone https://github.com/dreamhouseapp/dreamhouse-mobile-app
    ```
    
1. Navigate to the dreamhouse-mobile-app directory:
    ```
    cd dreamhouse-mobile-app
    ```

1. Install the dependencies
    ```
    npm install
    ```
    
## Build and Run in your Browser    

1. Install gulp
    ```
    npm install -g gulp
    ```

    or 
    
    ```
    sudo npm install -g gulp
    ```

1. Build the JavaScript app using the Ionic build script

    ```
    gulp build
    ```

1. Install force-server
    ```
    npm install -g force-server
    ```

    or

    ```
    sudo npm install -g force-server
    ```

1. Run the app in the browser
    ```
    force-server --root www
    ```
        
## Build and Run on Device    

1. Restore the state of the application using the `cordovaPlugins` and `cordovaPlatforms` entries in package.json:
    
    ```
    ionic state restore
    ```

1. Install the Mobile SDK plugin
    ```
    cordova plugin add https://github.com/forcedotcom/SalesforceMobileSDK-CordovaPlugin
    ```

1. Build the app for iOS
    ```
    ionic build ios
    ```

1. Open ```DreamHouse.xcodeproj``` in the ```dreamhouse-mobile-app/platforms/ios``` directory  

1. In Xcode, run the application, or select Product>Archive in the menu for App Store or Enterprise deployment