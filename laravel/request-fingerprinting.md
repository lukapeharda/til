# Request fingerprinting

In order to generate a unique identifier that will last a whole request we can use undocumented `$request->fingerprint()` method which outputs something like `cf3fcc20ae756f4d5a3e1f48a91e722ed93345ca`.
We can use this in our log messages in order to be able to trace a whole request.

See more [here](https://www.amitmerchant.com/request-fingerprinting-and-how-to-use-it-in-laravel).