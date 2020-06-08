# Payments Test Task

This is a small smoke test suite for the payments api located at https://github.com/eMerchantPay/codemonsters_api_full

In order to work with it the following prerequisites are required:

1. It needs to be downloaded locally in a Linux environment 
2. The ruby server needs to be initiated
3. The testing application must be invoked using the command line in the following format:
"ProjectFolder$ java -cp "dependencies/commonsio.jar:dependencies/json.jar" App.java -s"

The .jar dependencies must be included every time because this is a single file java application. 
The dependencies represent two java libraries necessary for the test (abbreviated for convenience):
commonsio.jar - org.apache.commons.io (https://mvnrepository.com/artifact/org.apache.commons.io/commonsIO)
json.jar - org.json (https://mvnrepository.com/artifact/org.json/json/20190722)

The app accepts the following command line arguments: <br />
-s    A successful transaction <br /> 
-v    A successful void of a transaction <br />
-ia   An unsuccessful transaction with an invalid authentication <br />
-vi   An unsuccessful void transaction with a non-existant purchase unique_id <br />
-vv   An unsuccessful void transaction attempting pointing to a successful previous void transaction <br />

Enjoy!
