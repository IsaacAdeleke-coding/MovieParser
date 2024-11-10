# MovieParser

MovieParser is a simple C++ project that parses a string in a specific format into a structured movie representation. Given a formatted string like `"24 s2,2014"`, it extracts the title, season, and year and stores them in a `Movie` struct. This is useful for applications that need to process and structure information about movies and TV shows.

## Project Structure


MovieParser/ ├── main.cpp # Entry point to the program for testing ├── MovieParser.cpp # Implementation of the parseMovieString function └── MovieParser.hpp # Header file defining the Movie struct and function declaration


## Files

- **MovieParser.hpp**: Contains the `Movie` struct definition and the declaration for the `parseMovieString` function.
- **MovieParser.cpp**: Implements the `parseMovieString` function, which parses a formatted string into a `Movie` struct.
- **main.cpp**: A sample test file that uses `parseMovieString` to demonstrate the parsing functionality.

## Usage

To run this project, compile it using `g++`:

```bash
g++ -o MovieParser main.cpp MovieParser.cpp

Then, execute the compiled binary:
./MovieParser
Example Input
The input to the parseMovieString function is a string formatted as follows:
"<title> s<season>,<year>"
Example:
std::string movieString = "24 s2,2014";
Expected Output
For the input "24 s2,2014", the program should output:
Title: 24
Season: 2
Year: 2014
Function Details

Movie parseMovieString(const std::string& movieString)
Description: This function takes a formatted string and parses it into a Movie struct containing the title, season, and year.
Parameters: A single std::string in the format "<title> s<season>,<year>".
Returns: A Movie struct with title, season, and year parsed from the input string.





