
<h1 align="center"> 🔷 Stock_Management 🔵 </h1>

This is a repository for the "Stock Management" application. The application focuses on managing stocks and provides various functionality to interact with the stocks. The main entity in this application is the "Stock" entity.



## Frameworks and Language used

[![JAVA Docs](https://img.shields.io/badge/JAVA-v20.0.1-blue.svg)](https://docs.oracle.com/en/java/)
[![GPLv3 License](https://img.shields.io/badge/Spring_Boot-v3.0.6-yellow.svg)](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/)


## Required Dependencies

To run this project, you will need to add the following dependencies to your pom.xml file

`Spring Web`,`Spring Boot Dev Tool`,`Lombok`,`Spring Data JPA`,`Validation`,`H2-DataBase`



## Controller Methods
`getAllStock`

This method is used to retrieve all available stocks in the system.

```bash
@GetMapping("/stocks")
public ResponseEntity<List<Stock>> getAllStock() {
    // Implementation code here
}
```

`getStockByName`

This method is used to retrieve a stock by its name.

```bash
@GetMapping("/stocks/{name}")
public ResponseEntity<Stock> getStockByName(@PathVariable String name) {
    // Implementation code here
}
```

`getAllByDateGreater`

This method is used to retrieve the stocks that have a release date after the given date.

```bash
@GetMapping("/stocks/releaseDate/{date}")
public ResponseEntity<List<Stock>> getAllByDateGreater(@PathVariable LocalDate date) {
    // Implementation code here
}
```

`insertStocks`

This method is used to add a new stock to the system.

```bash
@PostMapping("/stocks")
public ResponseEntity<Stock> insertStocks(@RequestBody Stock stock) {
    // Implementation code here
}
```

## Data Structure used in project :
- List

## Contributing
Contributions to the Stock Management application are welcome. If you encounter any issues or have suggestions for improvement, please feel free to open an issue or submit a pull request. Your contributions can help enhance the functionality and usability of the application.

## Project Summary :

````
  This is a Spring Boot project of basic Student portal system. Student can register themselves by filling the required information.
  Upon registration basic validation applied to the filled data if all the validation passes then and only then a data is registered into the system.
  Student can able to study by get some Course, Book etc, can look into all the courses, books. Whereas,
  Student can able to update their required information from the registered data using the Basic Student API.
  AtLast Student also can delete their account forever.
````

