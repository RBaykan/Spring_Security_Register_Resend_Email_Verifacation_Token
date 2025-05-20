# Spring Security Register Resend Email Verifacation Token

# Description
It is a continuation of the project linked here: https://github.com/RBaykan/Spring_Security_Register_Email_Verification_Token
A new verification token will be generated and sent via email for account verification.

## Steps to Run the Project
1. **Clone the repository**:
```bash
git clone https://github.com/RBaykan/Spring_Security_Register_Email_Verification_Token.git
```
2. **Navigate to the project directory**:
```bash
cd Spring_Security_Register_Resend_Email_Verifacation_Token
```
3. **Dependencies and build the project**:
```bash
mvn clean install
```
- Run the application:
```bash
mvn spring-boot:run
```
The application should now be running on `http://localhost:8080.`

4. To retrieve a new verification token for predefined users, send a `GET` request to:
  `http://localhost:8080/api/user/reSendRegistrationToken?email=user@usermail.com`

  This will invalidate the user's old verification tokens and generate a new verification token.
