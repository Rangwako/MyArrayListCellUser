# Cell Phone User Management System with Custom ArrayList and Sorting

This Java project extends the previous cell phone user management system by incorporating a custom `MyArrayList` class for storing user data and implementing sorting functionality based on the remaining minutes of users.

## Project Structure

The project is expected to consist of the following Java files:

*   `CellUser.java`: The superclass for all cell phone users, modified to support sorting.
*   `ContractUser.java`: A subclass extending `CellUser` for contract-based users.
*   `PrepaidUser.java`: A subclass extending `CellUser` for prepaid users, modified to support sorting based on minutes balance.
*   `MyArrayList.java`: The custom ArrayList class used to store `CellUser` objects.
*   `Driver.java`: A test program to demonstrate the functionality, including adding users to `MyArrayList` and sorting them.

## Features

*   Stores common details for all cell phone users (name, address, service provider, cell number).
*   Stores specific details for Prepaid users (data balance, minutes balance, amount balance).
*   Stores specific details for Contract users (contract start date, contract description, phone description, free minutes left, free SMSs left).
*   Includes `toString()` methods in each class (simplified for sorting demonstration).
*   Includes an abstract `showAccount()` method in the `CellUser` class, implemented by subclasses to provide formatted account details.
*   Utilizes a custom `MyArrayList` class for data storage.
*   Implements sorting of `CellUser` objects within the `MyArrayList` based on the remaining minutes (requires implementing the `Comparable` interface and a `compareTo` method in the relevant class, likely `CellUser` or `PrepaidUser` depending on your design).
*   A driver program to create and manage a `MyArrayList` of `CellUser` objects, add data, and demonstrate the sorting functionality.

## How to Compile and Run

1.  Save all the necessary Java files (`CellUser.java`, `ContractUser.java`, `PrepaidUser.java`, `MyArrayList.java`, `Driver.java`) in the same directory.
2.  Compile the Java files using a Java Development Kit (JDK). You can use the provided `run.bat` file on Windows or the following commands in a terminal:

    ```bash
    javac CellUser.java
    javac ContractUser.java
    javac PrepaidUser.java
    javac MyArrayList.java
    javac Driver.java
    ```

3.  Run the `Driver` program:

    ```bash
    java Driver
    ```

## `run.bat` (for Windows)

```batch
javac CellUser.java
javac ContractUser.java
javac PrepaidUSer.java
javac MyArrayList.java
javac Driver.java
java Driver
