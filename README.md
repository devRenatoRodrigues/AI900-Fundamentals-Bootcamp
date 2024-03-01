# ℹ️Dataset 
![Dataset](https://github.com/devRenatoRodrigues/car-price-predict/assets/115325126/8c20c273-f585-4f68-9ef5-ad060618a48b)

The objective of this repository is to document how to create a prediction model.

First we'll click in Automated ML then New Automated ML Job
![Automated ML Screen](https://github.com/devRenatoRodrigues/car-price-predict/assets/115325126/abc04116-646b-4d53-8fb6-934ccef314be)
Now we'll configure the service 
- **Job Name:** Car-predict-price
- **Experiment Name:** Create a New the name will be car-prices-predict

 **.......Next......**
 
- **Select task type:** Regression
- **Select data:** Create
- **I found my dataset on Kaggle after downloading it needs to be uploaded to Azure**
- **Name of dataset:** Car-infos
- **Data source:** From local Files
**In settings we'll select in column headers, Only first file has headers**

 **.......Next......**
 
- **Targe Column:** Price
- **Limits:** Expand this section
- **Max trials:** 3
- **Max concurrent trials:** 3
- **Max nodes:** 3
- **Timeout:** 15
- **Iteration timeout:** 15
- **Enable early termination:** Selected

**.......Next......**

- **Compute type:** Serveless
- **Virtual Machine** Type: CPU
- **Virtual Machine tier:** Dedicated
- **Virtual Machine Size:** Standard_DS3_V2
- **Instances:** 1

 **.......Review......**

  **Wait for the status is completed**

Now we'll go to the Job tab and select car-price-predict, and click in the algorithm name
![car-price-predict-screen](https://github.com/devRenatoRodrigues/car-price-predict/assets/115325126/326c1b10-e444-440e-abf0-a18c4fe3e20f)
Click in Deploy then Web Service 

**Coffee Break Time**

Go to the Endpoints tab, when the deployment status is healthy it means that everything went well

Now we have this to predict a price of car based in your Model, Price and Miles
![Result](https://github.com/devRenatoRodrigues/car-price-predict/assets/115325126/6efff1d0-2755-493c-b28e-ff8a3230c31d)


