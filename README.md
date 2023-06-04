# Setting Up PostgreSQL and PgAdmin Containers

This README guide will walk you through the process of setting up PostgreSQL and PgAdmin containers using Docker. By following these steps, you will be able to access the PgAdmin login and create a connection to the Project Manager database.

## Prerequisites

Before you begin, make sure you have the following requirements in place:

- Docker installed on your machine.

## Step 1: Start the Containers

1. Create a new directory for your project.
2. Create a file named `docker-compose.yml` in the project directory.
3. Copy and paste the provided docker-compose.yml configuration into the `docker-compose.yml` file.
4. Save the `docker-compose.yml` file.

## Step 2: Accessing PgAdmin Login

1. Open a web browser and enter the following URL: `http://localhost:5050`.
2. You will be directed to the PgAdmin login page.
3. Enter the following credentials:
   - Email: admin@admin.com
   - Password: root
4. Click on the "Sign in" button to log in to PgAdmin.

## Step 3: Creating a Connection to Project Manager Database

1. Once logged in to PgAdmin, navigate to the "Servers" section on the left sidebar.
2. Right-click on "Servers" and select "Create" and then "Server".
3. In the "Create - Server" dialog box, provide a name for your connection (e.g., Project Manager).
4. Under the "Connection" tab, enter the following details:
   - Host name/address: `pg_container`
   - Port: `5432`
   - Maintenance database: `project`
   - Username: `root`
   - Password: `root`
5. Click "Save" to add the server connection.
6. You should now see the newly created server connection under the "Servers" section.
7. Expand the server connection, and you will find the Project Manager database (`projectManager`) listed.

Congratulations! You have successfully set up the PostgreSQL and PgAdmin containers, accessed the PgAdmin login, and created a connection to the Project Manager database. You can now manage your database using PgAdmin.
