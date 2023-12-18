# MovieNITE Final Project

Movie suggestion app where users can provide their favorite movies and ChatGPT suggests a movie that everyone can enjoy. MovieNite is here to help you ease the process of decision-making with the help of Chat GPT. This project was a collaborative work from Levent and Neriman, and presented as the group's final project at the end of Lighthouse Labs Web Development Bootcamp in December 2023. 

## Project Structure

MovieNite has been built with React, Node.js, Express, and PostgreSQL in addition to MUI, HTML, CSS, and Chat GPT API. We implemented Json Web Token (JWT) for extra security and sending token from the front end to the back end to check if the users are already registered as well as to create a unique link to collect movie preferences and voted movie results from users via email that is generated with Nodemailer. We checked our backend routes and their functionalities with Postman to make sure everything worked as intended on the backend. We constructed 24 error cases and showed a couple of them in the app walkthrough. We built this app within the 3 weeks and we are working on adding more features. 

## Summary Of MovieNite

**Landing Page:**


- A user can log in to the app or register as an admin if not already. 

**Admin Dashboard:**


- Admin can create a group and add/delete members to it. Also, the admin can edit the group info or remove the entire group. 

- Admin can view their active and closed groups.

- Admin cannot remove themselves from their own group. 

- As soon as members are added to the group each member will receive an email to provide their three preferred movies. 

- Admin can see the near-real-time results on the dashboard after members submit their preferred movies. 

- After collecting movies, the admin sends them to Chat GPT to get three movie suggestions for each member can enjoy. 

- Admin will send the second email to group members to vote chat GPT suggestions.

- After voting is completed, the admin will get the result from the second email on the dashboard and let the group members know about the coming movie night. 

- Admin can log out from the app. 

## Screenshots
### Landing page
<img width="1680" alt="Screenshot 2023-12-16 at 1 37 32 PM" src="https://github.com/neridkmn/movie-nite/assets/128938408/aefd97cb-c6b6-4caa-a983-35847b9b2b85">

### Admin dashboard
<img width="1680" alt="Screenshot 2023-12-16 at 1 38 45 PM" src="https://github.com/neridkmn/movie-nite/assets/128938408/052fcb4f-1552-46fb-9d69-05321d95175e">

<img width="1680" alt="Screenshot 2023-12-16 at 1 39 31 PM" src="https://github.com/neridkmn/movie-nite/assets/128938408/773799fe-5694-4460-9342-3b1b4edc20b9">


### App walk-through Video
https://github.com/neridkmn/movie-nite/assets/128938408/82fcd3d1-f200-4042-85ee-50b95cc435da

### App walk-through GIF
![ezgif-3-f2c9f7e0dc](https://github.com/leventbk/movie-nite/assets/43709259/a8a4f70b-b001-4841-a634-e94ca91633a4)

## Getting Started

Please have two terminals open in your code editor as you need to start the back end and front end separately. 
  
1. CD in backend folder
2. Create the `.env` file using `.env.example` as a reference: `cp .env.example .env`
3. Update the `.env` file with your local database information:
   - username: `labber`
   - password: `labber`
   - database: `final`
   - JWT_SECRET_KEY = 123_ght
   - OPENAI_API_KEY=OPEN_AI_API_KEY_HERE
   - MAIL_AUTH_USER=example@example.com
   - MAIL_AUTH_PASS=MAIL_PASSWORD_HERE
   - MAIL_FROM=example@example.com
   - MAIL_TO=example@example.com
4. Install dependencies: `npm install`
5. Run psql in the terminal
    - Run `CREATE DATABASE final;`
    - Run `exit;`
6. Inside the backend folder reset the database: `npm run db:reset` (Note: This will reset data)
7. Run the server: `npm run nodemon`
   
8. CD in frontend folder
9. Install dependencies: `npm install`
10. Run the server: `npm start`

## Backend Dependencies

    "@types/express": "^4.17.20",
    "bcrypt": "^5.1.1",
    "body-parser": "^1.20.2",
    "chalk": "4.1.2",
    "dotenv": "^16.3.1",
    "express": "^4.18.2",
    "fs": "^0.0.1-security",
    "jsonwebtoken": "^9.0.2",
    "openai": "^4.14.1",
    "pg": "^8.11.3",
    "serverless-http": "^3.2.0",
    "uuid": "^9.0.1"
    "nodemon": "^3.0.1"

## Frontend Dependencies

    "@emotion/react": "^11.11.1",
    "@emotion/styled": "^11.11.0",
    "@mui/icons-material": "^5.14.18",
    "@mui/material": "^5.14.18",
    "@mui/styled-engine-sc": "^6.0.0-alpha.6",
    "@testing-library/jest-dom": "^5.17.0",
    "@testing-library/react": "^13.4.0",
    "@testing-library/user-event": "^13.5.0",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-router-dom": "^6.17.0",
    "react-scripts": "5.0.1",
    "styled-components": "^6.1.1",
    "web-vitals": "^2.1.4"
   
    
