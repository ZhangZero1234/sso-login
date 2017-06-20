How to launch the node server:
cd to the application directory
if you are not root: 
sudo node app >logs/access_log.txt 2>logs/error_log.txt
if you are root:
node app >logs/access_log.txt 2>logs/error_log.txt

Note: you can use nohup to run the node process in bacth
nohup node app >logs/access_log.txt 2>logs/error_log.txt &

Requirements:
npm install express
npm install formidable@latest
npm install passport
npm install passport-idaas-openidconnect --save
npm install express-session
npm install cookie-parser

URL:
https://x.xxx.xxx.xx/

object returned by authentication

{
    "id": "xxx@fr.ibm.com",
    "AUTHENTICATION_LEVEL": "0",
    "tenantId": "prepiam.toronto.ca.ibm.com",
    "_json": {
        "iss": "https://prepiam.toronto.ca.ibm.com",
        "ext": "{\"AUTHENTICATION_LEVEL\":\"0\",\"tenantId\":\"prepiam.toronto.ca.ibm.com\"}",
        "at_hash": "sdcdssdf3ete8QSQ",
        "sub": "xxx@fr.ibm.com",
        "realmName": "www.ibm.com",
        "uniqueSecurityName": "27154654SYB",
        "preferred_username": "xxx@fr.ibm.com",
        "given_name": "John",
        "aud": "ZEZDZDSSSdfs44",
        "exp": 1475510537,
        "iat": 1475506937,
        "family_name": "Thompson",
        "email": "xxx@fr.ibm.com"
    },
    "accessToken": "u45678646dqzdqzdqzzdfsqCOlffftFKAdWA7gVrN",
    "refreshToken": "fqsfdqsdqsdqszzefsetrsefg"
}


