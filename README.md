- š Hi, Iām @geoffgold9
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
geoffgold9/geoffgold9 is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

const speakeasy = require('speakeasy')
const qrcode = require('qrcode')


var secret = speakeasy.generateSecret({

    name: "Google"
})
qrcode.toDataURL(secret.otpauth_url, function(err, data){
    console.log(data)
})


