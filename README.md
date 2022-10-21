# openturnkey

OpenTurnKey is secure hardware storage for Bitcoin private keys which can be used to sign Bitcoin transactions.

The private key in an OpenTurnKey is randomly generated on its first boot-up as the root private key. The root private is only used to derive child keys and should not be used directly. A level 5th child key can be specified by the user or randomly chosen as M/(0~4294967296)/(0~4294967296)/(0~4294967296)/(0~4294967296)/(0~4294967296).

OpenTurnKey hardware design includes a fingerprint sensor. Whenever a user needs to access to the private key, i.e. sign a transaction, export the private key, etc., Only with valid fingerprint validation the access will be granted. 

NFC and wireless charging is used in OpenTurnKey to ensure the hardware will not be hacked via a physical connection. Only limited commands and data are allowed to be transmitted through NFC via a simple proprietary protocol. 

The hardware, firmware, and software of OpenTurnKey is published as an open-source design without any warranty. For anyone who is interested in making a product or personal use, please feel free to donwload the source. If there is any question, you may contact with me via GitHub or open an issue, but I cannot gauranttee to answer every one of them. 


OpenTurnKey firmware: https://github.com/Cyphereco/openturnkey-firmware

OpenTurnKey software: 
- for iOS: https://github.com/Cyphereco/openturnkey_app_ios
- for Android: https://github.com/Cyphereco/openturnkey-app-android
