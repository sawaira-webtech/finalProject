
Project Setup & Run Guide
1. Prerequisites
Ensure you have the following installed on your system:

Node.js (LTS version recommended)

npm (Node Package Manager)

MongoDB Account (for database)

Cloudinary Account (for image storage)

Firebase Account (for authentication/hosting)

PayPal/Razorpay Developer Accounts (for payments)

2. Server Configuration (Node.js/Express)
Navigate to the server directory:

Bash

cd "Fullstack ecommerce with admin with react and node new/updated code/server"
Install dependencies:

Bash

npm install
npm install express jsonwebtoken bcrypt
npm install -g nodemon
npm i --legacy-peer-deps

Environment Variables: Create a .env file in the server folder and paste the following:

Code snippet

PORT=8000
MONGODB_URI='mongodb+srv://awdcourse2025_db_user:awdcourse2024@nextgen.6tc2twe.mongodb.net/?appName=NextGen'
EMAIL=awd.course2025@gmail.com
EMAIL_PASS=fbuonabkxleditpx
JSON_WEB_TOKEN_SECRET_KEY=NextGen_string_here
SECRET_KEY_ACCESS_TOKEN=NextGen_string_here
SECRET_KEY_REFRESH_TOKEN=NextGen_string_here
cloudinary_Config_Cloud_Name="dsddwj8uo"
cloudinary_Config_api_key="382947629169341"
cloudinary_Config_api_secret="-6WITaM2jHSPJvs0JScufLPSkQI"
PAYPAL_MODE=dummy
PAYPAL_CLIENT_ID_TEST=dummy_client_id
PAYPAL_SECRET_TEST=dummy_secret
PAYPAL_BASE_URL=http://localhost:8000/payment
Run the Server:

Bash

nodemon index.js
3. Client Configuration (React/Vite)
Navigate to the client directory:

Bash

cd "Fullstack ecommerce with admin with react and node new/updated code/client"
Install dependencies:

Bash

npm install --legacy-peer-deps  //in index.js
npm install @mui/material @emotion/react @emotion/styled @mui/icons-material
npm install tailwindcss @tailwindcss/vite
Environment Variables: Create a .env file in the client folder:

Code snippet

VITE_API_URL=http://localhost:8000
VITE_FIREBASE_APP_API_KEY="AIzaSyCn3YNbCM46G3XjBHCmUe3_Tk9A5knk0nc"
VITE_FIREBASE_APP_AUTH_DOMAIN="ecommerce-b1579.firebaseapp.com"
VITE_FIREBASE_APP_PROJECT_ID="ecommerce-b1579"
VITE_FIREBASE_APP_STORAGE_BUCKET="ecommerce-b1579.firebasestorage.app"
VITE_FIREBASE_APP_MESSAGING_SENDER_ID="921449241894"
VITE_FIREBASE_APP_APP_ID="1:921449241894:web:231e778ae2e919a7fcb5e7"
Run the Client:

Bash

npm run dev
4. Admin Configuration (React/Vite)
Navigate to the admin directory:

Bash

cd "Fullstack ecommerce with admin with react and node new/updated code/admin"
Install dependencies:

Bash

npm install
npm install express jsonwebtoken bcrypt
npm install -g nodemon
npm i --legacy-peer-deps


Environment Variables: Create a .env file in the admin folder (similar to the client config).

Run the Admin Panel:

Bash

npm run dev
Important Service Links
MongoDB Atlas: https://www.mongodb.com/cloud/atlas (Manage your database clusters)

Cloudinary Dashboard: https://cloudinary.com/console (Manage product images)

Firebase Console: https://console.firebase.google.com/ (Manage Auth and Project Config)

PayPal Developer: https://developer.paypal.com/ (Manage Sandbox/Live credentials)

Razorpay Dashboard: https://dashboard.razorpay.com/ (Get your API Keys)

Project Scan Note
This is the project I want to talk about. I have scanned the file structure and identified the separate directories for admin, client, and server. Each component requires its own dependency installation and environment configuration as outlined above to ensure a correct run. If any part of the automated setup fails, please manually ensure the .env files are placed in their respective root directories.
