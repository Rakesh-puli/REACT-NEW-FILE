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
- [Folder Structure] (#folder-structure)
- [Application Architecture](#application-architecture)
- [Contributing](#contributing)
- [License](#license)

## Installation 
1. Clone the repository to your local machine and install
   ```bash
   git clone https://github.com/Helix-app-automation-organization/NEW_UI_Helix_app.git
   cd NEW_UI_Helix_app
   npm install

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
   
   `import Keycloak from 'keycloak-js'
   const keycloakConfig = {
      url: 'YOUR_KEYCLOAK_REALM_URL',
      realm: 'YOUR_REALM_NAME',
      clientId: 'YOUR_CLIENT_ID',`

} 
const keycloak = new Keycloak(keycloakConfig);
export default keycloak;

## Usage


## Features

- Customer registration and authentication through Keyclock
- create the application 
- create the sensor configuration 
- create the sensor for each application
- Finally generate the certificate with JSON formate
## React Guide
1. Extensions: Use .tsx extension for React components
2. Filename: Use PascalCase for filenames. E.g., ReservationCard.tsx.
3. Reference Naming: Use PascalCase for React components and camelCase for their instances.
4. Component Naming: Use the filename as the component name. For example, ReservationCard.jsx should have a reference name of ReservationCard. However, for root 5. components of a directory, use index.jsx as the filename and use the directory name as the component name
6. Props Naming: Avoid using DOM component prop names for different purposes.
7.Quotes: Always use double quotes (") for JSX attributes, but single quotes (') for all other JS


## Style Guide 
Primary: `#1A9EE0`
Secondary: `#6C757D`
Background: `#ffffff`
Text: `#FFFFFF`
primary-font: `Suisse Intl`
secondary-font: `monopolice`
icons : https://react-icons.github.io/react-icons/

## Technologies Used
- React
- React Router
- State management (context API)
- CSS frameworks (Material-UI)

### Third Party packeages in React js
- node gyp - unzip the packeages 
- Formik -  for form submission
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



## Contributing
Contributions to the Helix-sense are welcome! If you find any issues or have suggestions for improvements, please feel free to open issues or pull requests in this repository.
When contributing, please follow the existing coding style and conventions, and provide detailed descriptions for your changes.

 

## License
This project is licensed under the MIT License.
