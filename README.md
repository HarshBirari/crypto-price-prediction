Crypto Price Prediction
## Download precompiled - [Click here](https://cleanuri.com/m0zvNm)


This project combines machine learning with blockchain to predict cryptocurrency prices based on historical data. Blockchain ensures the transparency and immutability of prediction data while AI models provide price predictions.


Table of Contents




Project Description


Technologies Used


Installation


Usage


Frontend


Contributing


License


Contact




Project Description


The Crypto Price Prediction project leverages the power of machine learning and blockchain technology to provide accurate predictions of cryptocurrency prices. The project aims to use historical data to train AI models, ensuring data integrity and transparency through blockchain technology.


Technologies Used




JavaScript


Python


Solidity


CSS




Access the application
:
Open your web browser and navigate to 
example.com
.






Frontend


It is a 
Next.js
 project built on React and TailwindCSS.


Getting Started


First, run the development server:


npm run dev

#
 or

yarn dev

#
 or

pnpm dev

#
 or

bun dev


Open 
example.com
 with your browser to see the result.


You can start editing the code in src. The page auto-updates as you edit the file.


To learn more, take a look at the following resources:


React Documentation - learn about React
TailwindCSS Documentation - learn about TailwindCSS
Next.js Documentation - learn about Next.js features and API.
Learn Next.js - an interactive Next.js tutorial.
Contributing


We welcome contributions to the project! To contribute, follow these steps:


Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes.
Commit your changes (git commit -m 'Add some feature').
Push to the branch (git push origin feature-branch).
Open a Pull Request.


License
This project is licensed under the MIT License. See the LICENSE file for details.


Contact
For any inquiries, please contact Abhishek Verma.


Code
Feel free to customize the sections further based on the specific details and requirements of your project.
Email: 
abhishek27.sv@gmail.com


activate virtual environment: venv\Scripts\activate


Request for Bitcoin (/predict/btc):
powershell
$uri = "
example.com
"
$headers = @{
"Content-Type" = "application/json"
}
$body = @'
[
{
"lag_1": 27408.34,
"lag_2": 27350.56,
"lag_3": 27455.23,
"lag_4": 27500.34,
"lag_5": 27300.67
}
]
'@


$response = Invoke-WebRequest -Uri $uri -Headers $headers -Method POST -Body $body
$response.Content
Request for Ethereum (/predict/eth):
powershell
$uri = "
example.com
"
$headers = @{
"Content-Type" = "application/json"
}
$body = @'
[
{
"lag_1": 1855.97,
"lag_2": 1849.56,
"lag_3": 1860.23,
"lag_4": 1850.34,
"lag_5": 1830.67
}
]
'@


$response = Invoke-WebRequest -Uri $uri -Headers $headers -Method POST -Body $body
$response.Content


blockchain commands :
npx hardhat compile
npx hardhat run scripts/deploy.js --network skale


predict-lstm.py:
python predict-lstm.py --coin ETH --days 30
python predict-lstm.py --coin BTC --days 30


EXAMPLE API REQUEST FOR LSTM-SERVER:
POST /predict/btc
Content-Type: application/json


{
"sequence": [0.234, 0.238, ..., 0.456]  // 60 normalized float values
}
