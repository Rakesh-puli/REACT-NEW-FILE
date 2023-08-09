# Helix-sense Application


## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- 
## Features

- Customer registration and authentication through Keyclock
- create the application 
- create the sensor configuration 
- create the sensor for each application
- Finally generate the certificate with JSON formate

## Installation 
1. Clone the repository to your local machine and install
   ```bash
   git clone https://github.com/Helix-app-automation-organization/NEW_UI_Helix_app.git
   cd Helix-sense-application
   npm install
   npm start

Access the application in your browser at http://localhost:3010 or the specified port.

## Technologies Used
- React js 
- node js 
- Keycloak 
- Typescript
- Material UI

## Third Party packeages in React js
- node gyp - unzip the packeages 
- Formik -  for form submission
- antd -for design purpose

## Folder structure 
src/
|-- assets/
|   |-- images/
|   |-- styles/
|       |-- global.css
|
|-- components/
|   |-- Header/
|       |-- Header.tsx
|       |-- Header.css
|   |-- Sidebar/
|       |-- Sidebar.tsx
|       |-- Sidebar.css
|--  pages/
|     |-- Customers/
|        |-- Customers.tsx
|        |-- Customers.css
|
|    |-- Applications/
|        |-- Applications.tsx
|        |-- Applications.css
|
|    |-- Configuration/
|        |-- Configuration.tsx
|        |-- Configuration.css
|
|    |-- Sensors/
|        |-- Sensors.tsx
|        |-- Sensors.css
|
|    |-- Permissions/
|        |-- Permissions.tsx
|        |-- Permissions.css
|
|    |-- Dashboard/
|        |-- Dashboard.tsx
|        |-- Dashboard.css
|
|-- utils/
|   |-- api.ts
|
|-- App.tsx
|-- index.tsx



## Contributing
Contributions to the Helix-sense are welcome! If you find any issues or have suggestions for improvements, please feel free to open issues or pull requests in this repository.
When contributing, please follow the existing coding style and conventions, and provide detailed descriptions for your changes.

 

## License
This project is licensed under the MIT License.
