## Usage

```javascript
var  GigyaSDK  = require('gigyasdk'),
     Gigya     = new GigyaSDK({
         'apiKey' : '',
         'secret' : '',
         'ssl'    : true
     });

Gigya.services.socialize.getUserInfo({ 'uid' : '' }, function callback(error, result) {
    if (error) {
        // Gigya reported an error
        console.log(error);
    } else {
        // We have a valid user
        console.log(result);
    }
});
```