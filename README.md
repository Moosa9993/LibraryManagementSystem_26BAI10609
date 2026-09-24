# 📖 Community Library Catalog

A simple command-line application for managing a small library's book catalog. Built as a beginner-friendly Python project to practice core programming concepts like data structures, functions, loops, and user input handling.

## Project Overview

Community Library Catalog is a terminal-based inventory system that lets a user view, search, add, and manage the status of books in a library's collection. All data is stored in memory while the program runs, using a simple list of dictionaries to represent the book catalog — no external database required.

This project is a great starting point for understanding how small CRUD-style (Create, Read, Update, Delete) applications work before moving on to file storage, databases, or web interfaces.

## Features

- **View Catalog** — Displays all books in a clean, formatted table with ID, Title, Author, and Status.
- **Search Catalog** — Filter books by title or author (case-insensitive).
- **Add New Book** — Add a new book with title, author, and optional genre. New books default to "Available."
- **Manage Inventory**
  - Toggle a book's status between `Available` and `Checked Out`.
  - Delete a book from the catalog entirely.
- **Input Validation** — Gracefully handles invalid IDs or non-numeric input without crashing.
- **Clean Terminal UI** — Screen clears between actions for a more app-like experience.

## Technologies / Tools Used

- **Python 3** — Core programming language
- **Standard Library only:**
  - `os` — for clearing the terminal screen across platforms (Windows/macOS/Linux)
  - `sys` — for exiting the program cleanly

No external dependencies or packages are required.

## Steps to Install & Run the Project

### Prerequisites
- Python 3.7 or higher installed on your machine
- A terminal / command prompt

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/community-library-catalog.git
   ```
2. Navigate into the project folder:
   ```bash
   cd community-library-catalog
   ```
3. No additional dependencies to install — the project uses only Python's standard library.

### Running the Project

Run the script using Python:

```bash
python main.py
```

or, on some systems:

```bash
python3 main.py
```

You'll be greeted with the main menu:

```
[1] Search Catalog   [2] Add New Book   [3] Manage Book (Status/Delete)   [4] Exit
```

Follow the on-screen prompts to interact with the catalog.

## Instructions for Testing

This project doesn't currently include an automated test suite, but it can be manually tested by walking through each feature:

1. **Test viewing the catalog**
   - Run the program and confirm all starter books display correctly in the table.

2. **Test search**
   - Choose option `1`, search for a partial title (e.g., `hobbit`) and confirm only matching books appear.
   - Search for a term with no matches and confirm the "No books found" message appears.

3. **Test adding a book**
   - Choose option `2`, enter a title and author, and confirm the book appears in the catalog afterward.
   - Try submitting with an empty title or author and confirm it shows an error instead of adding a blank entry.

4. **Test managing inventory**
   - Choose option `3`, select a valid book ID, and toggle its status — confirm it switches between `Available` and `Checked Out`.
   - Select a valid book ID and delete it — confirm it no longer appears in the catalog.
   - Enter an invalid ID (e.g., `0`, a number too large, or letters) and confirm the program shows an error instead of crashing.

5. **Test exit**
   - Choose option `4` and confirm the program prints a goodbye message and closes.

> **Note:** For a more robust setup, consider adding automated tests with `pytest`, covering each function (`add_book`, `manage_inventory`, `show_catalog`) independently by refactoring user input out of the core logic.

## License

This project is open source and available under the [MIT License](LICENSE).
