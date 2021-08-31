

<img align="left" src="https://user-images.githubusercontent.com/62319355/123072323-0580e800-d448-11eb-87d2-0970736bef53.png" width="150" height="80" alt="PowerBI image">
<img align="right" src="https://user-images.githubusercontent.com/62319355/123382025-063e8900-d5c4-11eb-91bd-d22fa3213253.jpg" width="150" height="80" alt="cloudera logo">


:smile: :grinning: :sleepy: :relieved: :confused: :open_mouth: :astonished: :thumbsup:
# powerbi_odbc_cloudera_impala


```
Hi, in this repository, 
I am going to show you how to connect PowerBI and Cloudera Datalake Hue Impala.

There are two options.
(1) ODBC-based Method
(2) Impala Method

Before we start, please go to Cloudera Websites to download ODBC Impala connectors.

(HIVE is more robust for larger query but HIVE is slower than Impala.
https://www.cloudera.com/downloads/connectors/impala/odbc/2-6-0.html
https://www.cloudera.com/downloads/connectors/hive/odbc/2-6-1.html
```
#### Before you proceed, you might want to clear existing permissions.
#### This is because if you have previously attempted to establish connection and failed, you need to delete your previous configuration
<img align="center" src="https://user-images.githubusercontent.com/62319355/127885748-1f6857da-7a8c-4fe5-b2ad-1bca3b922bb4.png" width="450"  alt="Excel logo">

#### If you see an error message as shown above, you can clear data source settings by following the steps below
<img align="center" src="https://user-images.githubusercontent.com/62319355/127885756-34cc61f6-1cff-498a-a1e2-c70dcfb2f92f.png" width="450"  alt="Excel logo">
<img align="center" src="https://user-images.githubusercontent.com/62319355/127885767-ec8412ff-5e66-4274-b56a-ba7569bdb6e9.png" width="450"  alt="Excel logo">

#### Now let us return to the main topic



# Option 1. ODBC-based Method
### ODBC-based method has embedded impala connection

### You can establish connection as shown below  :thumbsup:
<img align="center" src="https://user-images.githubusercontent.com/62319355/104537551-22252280-5655-11eb-9ea0-4de6e27e0114.png" width="450"  alt="ODBC impala">

### Please enable SSL Certifcate as shown below.
<img align="center" src="https://user-images.githubusercontent.com/62319355/104538259-7e3c7680-5656-11eb-84c0-0bb1ded086e1.png"   alt="SSL">

```diff
+ Now we will connect PowerBI to ODBC
```
### Choose ODBC as your data source
<img align="center" src="https://user-images.githubusercontent.com/62319355/123384834-713d8f00-d5c7-11eb-9713-16f1103f896b.PNG"   alt="ODBC_step_1">
<img align="center" src="https://user-images.githubusercontent.com/62319355/123385451-1f493900-d5c8-11eb-8bbf-684c29909483.PNG"   alt="ODBC_step_2">
<img align="center" src="https://user-images.githubusercontent.com/62319355/123386227-01300880-d5c9-11eb-9dc6-5ccf6d033699.PNG"   alt="ODBC_step_3">

### Transform your data and load the data
<img align="center" src="https://user-images.githubusercontent.com/62319355/123821992-77689e00-d92e-11eb-9ac1-ba4e2c65da50.PNG"   alt="ODBC_step_3">

```diff
- Before you load the data, make sure you only choose required columns. 
Otherwise, it might take forever to load data
- Still, it is going to take some time to load your data depending on the sources
```

### Once you have loaded the data, you can proceed to create visuals


# Option 2. Impala Method
### Choose Impala as your data source
<img align="center" src="https://user-images.githubusercontent.com/62319355/131309178-2ad5097f-3080-4d14-8c0a-571e364e9ec1.PNG" width="450"  alt="Impala">


### Input the url address of Impala server
#### you might want to ensure that the url does not contain leading "https://"
<img align="center" src="https://user-images.githubusercontent.com/62319355/131434698-51ba28ad-1dd7-4ef1-be3a-5492b751574a.png" width="450"  alt="Impala">

### Use Windows Credential
<img align="center" src="https://user-images.githubusercontent.com/62319355/131435091-986fa3f1-16ab-4c76-9d2d-a037a4af686e.png" width="450"  alt="Impala">

```diff
- Before you load the data, make sure you only choose required columns. 
Otherwise, it might take forever to load data
- Still, it is going to take some time to load your data depending on the sources
```

### Once you have loaded the data, you can proceed to create visuals

![image](https://user-images.githubusercontent.com/62319355/131435723-7831b12a-80b2-45dc-bc05-7be7523784e5.png)




# The END

