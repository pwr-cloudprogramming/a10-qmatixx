# Contigo App with AWS Cognito Protection

**Name:** Khalid Muzaffar  
**Group:** Group 3  
**Date:** 25-Apr-2024

## Objective
Protect your application using AWS Cognito.

## Requirements

### Backend
- **Authorization and Authentication**: Implemented using AWS Cognito.
- **Dependencies**: Added the necessary dependencies for AWS SDK and Cognito API.
- **Authentication Service**: Created a service to verify user authentication data using the AWS SDK or directly the Cognito API interfaces.
- **Endpoint Security**: Defined which endpoints are public and which require authorization using Spring Security configuration.

### Frontend
- **SDK Configuration**: Configured the SDK to connect with the user pool in AWS Cognito.
- **Registration Form**: Created a form to collect username, email address, and password.
- **Login Form**: Created a form to collect username and password.
- **Token Management**: Implemented logic to save access and refresh tokens in localStorage after successful login.
- **Token Refresh**: Implemented logic to automatically refresh the access token using the refresh token.
- **Request Authentication**: Automatically appended access tokens to requests sent to the backend.
- **Logout Function**: Implemented a function to clear user session data, including tokens stored in the browser, and optionally inform Cognito about the end of the session.

## Architecture

### Components
- **VPC**: Custom Virtual Private Cloud to provide an isolated network environment.
- **Subnets**: Public subnet to host the EC2 instance, enabling external access.
- **Route Tables**: Configurations to define rules and routes to control the traffic flow.
- **Security Groups**: Defined to allow ingress traffic on ports 22 (SSH), 80 (HTTP), and 8080 (HTTP for backend services) and egress traffic to all destinations.
- **EC2 Instance**: AWS EC2 instance running Ubuntu, with Docker installed to containerize the Contigo application's frontend and backend.
- **AWS Cognito**: Managed user pool and identity pool to handle user authentication and authorization.

## Preview

### Configured AWS Services

Teraaform Ec2 Instance
![image](https://github.com/pwr-cloudprogramming/a10-KhalidMuzaffar269553/assets/149905898/38f121f2-be4e-4b80-aea8-19b325c61c1c)

User pool:
![image](https://github.com/pwr-cloudprogramming/a10-KhalidMuzaffar269553/assets/149905898/858d7f50-d09c-4860-aa60-409a122f7ef1)

config.js
![image](https://github.com/pwr-cloudprogramming/a10-KhalidMuzaffar269553/assets/149905898/f191036e-780b-4912-bcf2-fdf1993d007c)

authservies.js
![image](https://github.com/pwr-cloudprogramming/a10-KhalidMuzaffar269553/assets/149905898/885f2943-2e0c-4d20-8fd9-17198a1c8c68)



### Application Running

![image](https://github.com/pwr-cloudprogramming/a10-KhalidMuzaffar269553/assets/149905898/dd348d5d-45f0-49e7-9c7f-9bc1cabd552e)


## Reflections

### Learning Outcomes
- Learned how to integrate AWS Cognito for user authentication and authorization.
- Gained experience in configuring AWS services and securing application endpoints with Spring Security.
- Enhanced understanding of managing tokens and user sessions on the frontend.

### Challenges
- Initially faced difficulties in configuring AWS Cognito and integrating it with the application.
- Handling token refresh and ensuring secure storage and transmission of tokens required careful implementation.
- Setting up secure and efficient communication between the frontend and backend, including proper handling of authentication headers.



### Surprises
- The comprehensive set of features provided by AWS Cognito for managing user authentication and authorization.
- The ease of configuring and managing security groups in AWS to control access to the application.
- The power of Spring Security in defining and managing access control for application endpoints.

