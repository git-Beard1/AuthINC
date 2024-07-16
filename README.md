# AUTHINC Boiler Template

## Introduction

AUTHINC is a robust authentication service, providing a comprehensive user management solution for your applications. It offers a streamlined and secure way to handle user registration, login, authentication, and authorization. This repository serves as a boiler template for the AY23/24 ProjectINC to start development. This template is done by **Group 4: Authentication and Authorization**.

## Tech Stack

### Frontend
- React + Vite
- Shadcn
- Tailwind

### Backend
- NodeJS
- Express
- JWT Token
- PostgreSQL
- Prisma ORM

## Getting Started

1. Run **npm i** at the client and server root directories respectively to install all dependencies.

2. Add **.env** file at the server directory and add in the the usable port and shared Neon databaseURL. 

3. Run **npm run dev** for nodemon, or **npm start** for node to start server for both frontend and backend.

4. After building the postgreSQL schema, run **npx prisma db pull** to convert to prisma schema. Check prisma.schema file for changes under *primsa* folder.

5. Run **npx prisma generate** to generate a new prisma client to apply changes and interact with the database.

6. If a schema is to be made directly with prisma syntax, update the model in schema.prisma file and run **prisma migrate dev** to keep logs and revert back to the previous model. 

7. Run **npx prisma db push** to apply changes in the main database: postgreSQL.

8. Data fetching to be done with **axios**.

### Note
Changes to schema models will wipe out all data if **npx prisma db pull** is implemented. Do make sure to backup database or restart database.
