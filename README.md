# KATA ORDER IMPORT

This application is developed with Spring Boot to handle the import of data from a list of online order requests from an external API to a relational database. Additionally, the application supports the export of data to a CSV file.

## Prerequisites
Before running the application, ensure that you have the following installed:

- Java JDK 17 or higher
- Maven
- PostgreSQL Database

## Configuration
- Clone this repository: `https://github.com/anagboc/kata_importer.git`
- Navigate to the project directory: `cd kataorderimporter`
- Set up the PostgreSQL database according to the application's requirements.(application.properties)
- Compile the project: `mvn clean install`

## Test
Run the application: `mvn test`

## Execution
Run the application: `mvn spring-boot:run`


# Technical Information
Objective
Import a list of online orders into a database.

Details
The list of orders is available in a public REST API.
The application queries the API to retrieve all orders to import.
It imports the data into a PostgreSQL database.
Upon completion of the import, it displays a summary of the number of orders of each type based on different columns.
It generates a CSV file with records sorted by order number.
Exported File Format
The resulting CSV file has the following columns:

Order ID
Order Priority
Order Date
Region
Country
Item Type
Sales Channel
Ship Date
Units Sold
Unit Price
Unit Cost
Total Revenue
Total Cost
Total Profit

Dates are displayed in the format: "{day}/{month}/{year}".

