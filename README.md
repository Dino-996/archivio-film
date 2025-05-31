# Library Rental System

A Java application for managing book rentals in a library, built with Vaadin and Spring Boot.

## Features

### Use Cases Implemented

1. **Operator Loads Archive**
   - Load library data (mock object or JSON file)
   - For intermediate level: Load from JSON file selected by operator

2. **Operator Searches Users**
   - Search users by name and/or surname (both fields optional)
   - Display results in table with:
     - Username, name, surname
     - Total books borrowed
     - Books currently on loan
   - Results ordered by total books borrowed (ascending), then by current loans (ascending)

3. **Operator Manages Rentals**
   - Select a user to view details
   - Show books borrowed grouped by author (ordered by count descending)
   - Add new rental (book title, author, start date)
   - Automatic return handling if user has >3 unreturned books
   - Error handling for invalid data

4. **Operator Verifies Archive**
   - Check books borrowed >6 months ago and not returned
   - Verify if all such books have distinct authors
   - Display verification result

5. **Intermediate Level Features**
   - Find author with highest average rental duration
   - JSON archive loading functionality

## Technical Details

- **Framework**: Vaadin + Spring Boot
- **Build System**: Gradle
- **Testing**: JUnit 5
- **Logging**: SLF4J + Logback
- **Lombok**: For boilerplate reduction

## Dependencies

- Spring Boot Starter Web
- Vaadin
- SLF4J API
- Logback Classic
- JUnit Jupiter
- Lombok

## How to Run

1. Build with Gradle
2. Run Spring Boot application
3. Access UI at `http://localhost:8080`

## Project Structure

- `src/main/java`: Application code (MVC structure)
- `src/test/java`: Unit tests
- `src/main/resources`: Configuration files
