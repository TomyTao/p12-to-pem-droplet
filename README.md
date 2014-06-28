p12-to-pem-droplet
==================

Simple Apple Script Droplet that converts .p12 files (from APNS &mdash; Apple Push Notifications Service) to .pem format. 

## How to Use 

- Clone repo 
- open P12toPEM.scpt in AppleScript Editor
- Choose File -> Export, select File Format: Application, save app 
- Drag and drop your p12 file to resulting Application 
- .pem file will be created in the same dir 


## Why 

People often use Keychain Access app on Mac to generate private key, certificate request and import certificate. 

OpenSSL-based solutions for sending push messages (Uniqush, Apns-PHP, etc) require certificate and private key to be in PEM format. 

Convertion could be done using openssl command line, but GUI may be simplier. 


## Known Issues 

- Only p12 files with empty password are supported 
