# Helix-sense Application

## Description 

HelixSense is an innovative project that aims to revolutionize the way sensor configurations are implemented in electrical systems. In a rapidly advancing technological landscape, the need for efficient and intelligent solutions for managing electrical devices and systems is paramount.

## Table of Contents
- [Installation](#installation)
- [Usage](#Usage)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [React Guide](#React-guide)
- [Style Guide](#Style-guide)
- [Folder Structure](#folder-structure)
- [Application Architecture](#application-architecture)
- [Contributing](#contributing)
- [License](#license)

## Installation 
1. Clone the repository to your local machine and install
   ```
   bash
   git clone https://github.com/Helix-app-automation-organization/NEW_UI_Helix_app.git
   cd NEW_UI_Helix_app
   npm install
   ```

 ## Introduction to Keycloak

Keycloak is an open-source Identity and Access Management (IAM) solution that provides robust authentication, Single Sign-On (SSO), authorization, and other security features for web applications and services. It allows you to easily add security measures to your applications without needing to reinvent the wheel, making it an excellent choice for projects that require user authentication and authorization.

### Main Features of Keycloak

- **Authentication**: Keycloak supports various authentication methods including username/password, social logins, multi-factor authentication (MFA), and more.

- **Single Sign-On (SSO)**: Users can authenticate once and then access multiple applications without needing to log in again.

- **Authorization and Role-Based Access Control**: Keycloak provides role-based access control, allowing you to define fine-grained permissions for different user roles.

- **Token-Based Security**: Keycloak issues JSON Web Tokens (JWTs) that can be used to securely transmit user information and permissions between services.

- **Client-Side Adapters**: Keycloak offers client-side adapters for various programming languages and frameworks, making it easy to integrate authentication into your applications.

### Why Use Keycloak

Keycloak simplifies the process of adding authentication and authorization to your applications, saving development time and ensuring best practices in security. By leveraging Keycloak, you can focus on building your application's core features while leaving the complex aspects of security to the experts.

## Installation and Authentication Setup with Keycloak
### Step 1: Install Keycloak
1. Download Keycloak: Visit the [Keycloak Download](https://www.keycloak.org/documentation.html) page and download the latest version of Keycloak.
2. Extract Keycloak: Extract the downloaded archive to a directory of your choice.
3. Access Keycloak Admin Console: Open your web browser and navigate to  http://localhost:8080/auth/admin. This is the Keycloak Admin Console where you will configure your realm, clients, roles, and more.


### Step 2: Configure Keycloak Realm
Login: Log in to the Keycloak Admin Console using the default admin credentials:
Username: admin
Password: admin
Create a Realm: Click on the Add realm button to create a new realm for your application. Give it a name and save.
Create a Client: Inside your newly created realm, go to the Clients tab and click Create.
Give your client a name.
Set the Client Protocol to openid-connect.
Click Save.

### Step 3: Configure Your React App
1. Install Required Packages: In your React project directory, install this package for integrating Keycloak:
``` npm install keycloak-js @react-keycloak/web. ```
2. Create Keycloak Configuration: Create a file named keycloak.js in your project's source directory.
   ```
   import Keycloak from 'keycloak-js'
   const keycloakConfig = {
      url: 'http://13.213.201.186:8080/auth/',
      realm: 'Dashboard',
      clientId: 'React-app',
   } 
   const keycloak = new Keycloak(keycloakConfig);
   export default keycloak
    ```
## Usage
1. The HelixSense user interface provides a user-friendly environment for sensor
configuration. Here's how you can configure sensors:
 -  Log in to the HelixSense platform using your credentials.
 -  **Customers**:
   This section might display a list of customers, their information, and possibly allow users to perform actions related to customers, such as viewing details 
   or managing customer data.
 -  **Configurations**:
   The configurations section could include Sensor code and Sensor Type  can be configure for your application. 
 -  **Applications**:
   The applications section could involve displaying a list of installed applications, We can Create the application and  give access also.  
 -  **Sensors**:
   In the sensors section, you might display list  sensors, their respective Applications. we can add the sensor for each application.

## Features

- **Sensor Data Collection**:
IoT sensors placed in different rooms detect motion, light levels, and temperature. These sensors continuously collect data and transmit it wirelessly to a central data hub.
-  **Data Processing**:
The central hub aggregates and processes the incoming sensor data. It analyzes motion patterns, light levels, and temperature changes to determine occupancy status and environmental conditions.
-  **Decision Logic**:
Based on the processed sensor data, the system's decision-making logic determines whether a room is occupied, the level of lighting required, and the optimal temperature settings.
-  **Control Commands**:
Once the decision logic is applied, the system generates control commands. For example, if no motion is detected for a certain period, the system may send a command to turn off lights and adjust AC settings.
-  **Device Communication**:
The control commands are sent to IoT devices such as smart switches for lights and smart thermostats for ACs. These devices receive and execute the commands to control the lighting and temperature in the rooms.
-  **User Interaction**:
Users can interact with the system through a mobile app or other interfaces. They can override automatic controls, adjust schedules, or monitor energy consumption remotely.

-  **Real-time Monitoring**:
Users can monitor the real-time status of rooms through the user interface. They can see occupancy status, lighting levels, and temperature settings.
As the number of IoT sensors increases or new rooms are added, the system's architecture should be designed to handle the growing volume of data and control commands.
## React Guide
1. Extensions: Use .tsx extension for React components
2. Filename: Use PascalCase for filenames. E.g., ReservationCard.tsx.
3. Reference Naming: Use PascalCase for React components and camelCase for their instances.
4. Component Naming: Use the filename as the component name. For example, ReservationCard.jsx should have a reference name of ReservationCard. However, for root 5. components of a directory, use index.jsx as the filename and use the directory name as the component name
6. Props Naming: Avoid using DOM component prop names for different purposes.
7.Quotes: Always use double quotes (") for JSX attributes, but single quotes (') for all other JS


## Style Guide 
```
Primary: `#1A9EE0`
Secondary: `#6C757D`
Background: `#ffffff`
Text: `#FFFFFF`
primary-font: `Suisse Intl`
secondary-font: `monopolice`
```
icons : https://react-icons.github.io/react-icons/

## Technologies Used
- React
- Keycloak 
- React Router
- State management (context API)
- CSS frameworks (Material-UI)

### Third Party packeages in React js
- node gyp - unzip the packeages 
- Formik -  for form submission & validation
- antd -for design purpose

## Folder structure   
```
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
  ```
## Application Architecture
![.](https://user-images.githubusercontent.com/111567733/259751506-8ddfa9b9-0335-49a2-8b41-6d5bfc362aed.png)


## Contributing
Sai Rakesh Puli  : git - Rakesh-puli

 

## License
Sai Rakesh Puli email:  Rakesh.puli@tynybay.com
