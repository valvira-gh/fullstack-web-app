# Fullstack Web App

## Description

This is a learning project that focuses mostly on _Docker_, but also:

- Postgres
- pgAdmin
- Node.js
- Next.js

## How to use

This application is _not yet_ ready for use outside of my learning goals.

## Form of this README

This README service purpose of being a manual of different topics for me. After this the Guide part begins:

## How to use Postgres and pgAdmin?

### Configuration

.env

Before deploying this setup, you need to configure the following values in the .env file.

    POSTGRES_USER
    POSTGRES_PW
    POSTGRES_DB (can be default value)
    PGADMIN_MAIL
    PGADMIN_PW

### How to use pgAdmin

- After the compose, pgAdmin is available at http://localhost:5050.
- Sign-in using the email and the password you've initialized at .env-file.
- Right-click "Servers" -> "Register" -> "Server..."
- Give a name to the server, then go to "Connection" tab
- Give Host name/address the name of the container of your postgres db (e.g. "postgres" or "db")
- Port: 5432
- Maintenance database: ${POSTGRES_DB} @ .env
- Username: ${POSTGRES_USERNAME} @ .env
- Password: ${POSTGRES_PW} @ .env
