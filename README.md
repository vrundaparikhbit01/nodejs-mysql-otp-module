
## Requirements / Packages Dependencies:

- Need to install these packages - express cors dotenv nodemailer mysql
  (npm install express cors dotenv nodemailer mysql --save)

## Configurations:

- Copy .env.example file to .env file and change Database details and Mail details as per your project.

## Database (Mysql) Requirements

- Database table name must be "users" which must contains atleast "email, otp, otp_expire_time" fields. (Attatching db sql file for reference - nodejs-mysql-otp-module.sql)

## Copy app folder and server.js file.

## API Details:

1. get-otp

	- URL: http://localhost:8080/user/common/get-otp
	- Method: POST
	- Required Parameters: email

2. verify-otp

	- URL: http://localhost:8080/user/common/verify-otp   
	- Method: POST
	- Required Parameters: email, otp