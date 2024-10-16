# 0x06. Star Wars API

## Description

This project involves interacting with the **Star Wars API** to fetch and display information about Star Wars characters based on the movie ID provided as a command-line argument. The script will retrieve character data from the API and print each character's name in the order they appear in the "characters" list of the given movie.

## Learning Objectives

The key concepts covered in this project include:

- **HTTP Requests in JavaScript**: Using modules like `request` to make HTTP requests to external services.
- **Working with APIs**: Understanding how to interact with RESTful APIs and handle JSON responses.
- **Asynchronous Programming**: Managing asynchronous operations with callbacks, promises, and async/await.
- **Command Line Arguments in Node.js**: Accessing and processing command-line arguments using `process.argv`.
- **Array Manipulation**: Iterating through arrays and manipulating data structures to format and display character names.

## Requirements

- All files must be interpreted on **Ubuntu 20.04 LTS** using **Node.js** version 10.14.x.
- The first line of all your files should be `#!/usr/bin/node`.
- Your code must be **semistandard compliant** (Standard + semicolons).
- All files should end with a new line.
- No use of `var` (use `const` or `let`).
- All files must be executable.
- The length of your files will be tested using `wc`.

## Project Structure

```bash
.
├── 0-starwars_characters.js   # Main script to fetch and display Star Wars characters
├── README.md                  # Project documentation


$ ./0-starwars_characters.js 3
Luke Skywalker
C-3PO
R2-D2
Darth Vader
Leia Organa
Obi-Wan Kenobi
Chewbacca
Han Solo
Jabba Desilijic Tiure
Wedge Antilles
Yoda
Palpatine
Boba Fett
Lando Calrissian
Ackbar
Mon Mothma
Arvel Crynyd
Wicket Systri Warrick
Nien Nunb
Bib Fortuna
```
