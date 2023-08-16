# Helix-sense Application

## Description 

HelixSense is an innovative project that aims to revolutionize the way sensor configurations are implemented in electrical systems. In a rapidly advancing technological landscape, the need for efficient and intelligent solutions for managing electrical devices and systems is paramount.

## Table of Contents
- [Installation](#installation)
- [Usage](#Usage)
- [Features](#features)
- [Technologies Used](#technologies-used)
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
Download Keycloak: Visit the [Keycloak Download] page and download the latest version of Keycloak.

Extract Keycloak: Extract the downloaded archive to a directory of your choice.

Start Keycloak: Navigate to the extracted directory and run Keycloak using the following command:

sh
Copy code
```bin/standalone.sh
This will start the Keycloak server.

```python
def greet(name):
    return f"Hello, {name}!"

Access Keycloak Admin Console: Open your web browser and navigate to http://localhost:8080/auth/admin. This is the Keycloak Admin Console where you will configure your realm, clients, roles, and more.

## Features

- Customer registration and authentication through Keyclock
- create the application 
- create the sensor configuration 
- create the sensor for each application
- Finally generate the certificate with JSON formate

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
