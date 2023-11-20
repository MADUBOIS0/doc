---
eleventyComputed:
  title: Two-Step Verification
  keywords:
  - 2 factor
  - 2FA
  - authentication
  - MFA
---
Add a layer of security to your {{ en.DA }} by setting up a two-step verification (2FA) method.  

## Account recovery configuration 

1. Connect to your {{ en.DA }} and click ***Two-Step Verification***.  
![!!Cloud4028](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4028.png) 
1. Click ***Configure***. 
1. Choose your account recovery method between ***SMS*** or ***Email***. 
![Two-Step Verification Step 1](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4029.png) 
1. Enter either your phone number or email address, click ***Send***.
![SMS Recovery Method](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4030.png) 
1. Enter the 6-digit code received in the chosen method (Step 3) then ***Next***. 

## Recovery codes 

Recovery codes are used to access your account as a last resort. You will be able to regenerate them once the configuration process is completed. This step is mandatory for security reasons.  

***Download*** or ***Print*** the recovery codes in a safe accessible place. Click ***Next***.  

![Recovery Codes](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4031.png) 

### Two-Step Verification Configuration 

On logging in, your authenticator app will prompt you to verify through a push notification.  

Choose <a href="#push">Authenticator Push</a>, <a href="#app">Authenticator App</a> or <a href="#key">Security Key</a> to configure the verification of your account.  

## Authenticator push <a name="push"></a>

1. Click ***Authenticator Push***.  
![Authenticator Push](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4032.png) 
1. Download and install the {{ en.WAPP }} on your mobile device.  
![{{ en.WMAPP }}](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4034.png)
1. Use {{ en.WAPP }} to scan the barcode or enter manually the code.
![{{ en.WS }} Barcode Scan](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4036.png)
1. Wait for app synchronization and pairing request on the mobile device. Accept the pairing request, click ***Complete***.  
![Application Synchronization](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4039.png)

## Authenticator app <a name="app"></a>

1. Click ***Authenticator App***.  
![Authenticator App](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4033.png)
1. Download and install an Authenticator App on your mobile device.  
![Authenticator App Download](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4035.png)
1. Use your authenticator app to scan the barcode or enter manually the code.
![Authenticator Barcode Scan](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4037.png)
1. Enter the 6-digit code generated by the authenticator app, click ***Activate*** then ***Complete***.
![Authenticator App Code](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4038.png)

## Security key <a name="key"></a>

1. Click ***Security Key***.  
![!!Cloud4048](https://webdevolutions.azureedge.net/docs/en/cloud/Cloud4048.png) 
1. You will be redirected to the [Security Key](/cloud/sign-in-security/security-key/) section of the {{ en.DA }}. 