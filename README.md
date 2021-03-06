# JShell Scripting

Samples for scripting with Java 10 and JShell.

## Requirements
- OpenJDK 10 or any other JDK 10 containing JShell
- A text editor

## Structure
This project is split in different folders:

- encoding (Base64, Hex, ...)
- files (working with files and folders)
- httpclient (working with the new http client)
- misc (params via system properties, ...)

## Work on this project
If you find a bug or think a script should be included, you're gladely invited to create a pull request!


## Third party libraries
The JShell scripting repo currently contains some well-known and very useful third party libraries like Apache Commons Lang 3. Those libraries and their PGP signatures are checked in to the repo for ease of use. The version numbers are removed from the file name for easy upgradability, but can be found within the manifest of the corresponding Jar.

### Verify the signatures of the third party libraries
1. Import the [PGP keys](https://www.apache.org/dist/commons/KEYS) of the Apache Foundation 
2. Verify each library (in `libs` folder) with their signature (e.g. `gpg --verify commons-lang3.jar.asc`)