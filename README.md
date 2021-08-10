- 👋 Hi, I’m @geoffgold9
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
geoffgold9/geoffgold9 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
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


