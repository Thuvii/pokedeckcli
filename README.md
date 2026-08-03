# Pokédex CLI

A command-line REPL application for exploring the Pokémon world.

A **Pokédex** is a fictional device that stores information about Pokémon, including their names, types, stats, and other characteristics. This project allows users to explore locations, discover Pokémon, catch them, and build their own personal Pokédex directly from the terminal.

> **Note:** This project was built by following the Boot.dev backend course and serves as a learning project for building command-line applications in Go.

---

## Features

* Interactive command-line REPL
* Explore Pokémon locations
* Fetch Pokémon and location data from the PokeAPI
* Built-in API response caching to reduce repeated requests
* Discover Pokémon available in each area
* Catch Pokémon and add them to your personal Pokédex
* Inspect detailed Pokémon statistics
* View all Pokémon you've caught
* Simple command system with built-in help and exit commands
* Written entirely in Go using the standard library and HTTP requests

---

## Tech Stack

| Category   | Technology               |
| ---------- | ------------------------ |
| Language   | Go 1.22+                 |
| API        | PokeAPI                  |
| Interface  | Command-Line (REPL)      |
| Networking | Go `net/http`            |
| Caching    | In-memory response cache |

---

# Getting Started

## Prerequisites

* Go 1.22.2 or later

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/Thuvii/pokedeckcli.git
cd pokedeckcli
```

### 2. Install dependencies

```bash
go mod download
```

### 3. Build the application

```bash
go build -o pokedex
```

### 4. Run the application

```bash
./pokedex
```

---

# Available Commands

| Command              | Description                                         |
| -------------------- | --------------------------------------------------- |
| `help`               | Display all available commands                      |
| `exit`               | Exit the Pokédex                                    |
| `map`                | Display the next 20 map locations                   |
| `mapb`               | Display the previous 20 map locations               |
| `explore <location>` | Explore a location and list the Pokémon found there |
| `catch <pokemon>`    | Attempt to catch a Pokémon                          |
| `inspect <pokemon>`  | Display detailed information about a caught Pokémon |
| `pokedex`            | Show every Pokémon you've caught                    |

---

# Example Session

```text
Pokedex > map

canalave-city-area
eterna-city-area
...
20 locations displayed

Pokedex > explore canalave-city-area

Found Pokémon:
- Tentacool
- Wingull
- Pelipper

Pokedex > catch wingull

Throwing a Poké Ball at Wingull...
Wingull was caught!

Pokedex > inspect wingull

Name: Wingull
Height: 6
Weight: 95
Types:
  - Water
  - Flying

Pokedex > pokedex

Your Pokédex:
- Wingull
```

---

# Learning Objectives

This project was created to practice:

* Building interactive CLI applications
* Implementing a REPL in Go
* Working with REST APIs
* Making HTTP requests using the Go standard library
* Parsing JSON responses
* Managing application state
* Implementing in-memory caching
* Organizing Go projects into reusable packages

---

# API

This project uses the free **PokeAPI** to retrieve Pokémon and location information.

https://pokeapi.co/

---

# Acknowledgments

* Boot.dev for the project tutorial
* PokeAPI for providing a free Pokémon REST API
* The Go community for its excellent tooling and libraries

---

## Author

**Thuvii**

GitHub: [@Thuvii](https://github.com/Thuvii)

---

## License

This project is intended for educational purposes.

---

⭐ If you found this project helpful, consider giving it a star on GitHub!
