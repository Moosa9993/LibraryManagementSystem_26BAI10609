# Project Statement — Library Management System

## Problem Statement

Small libraries, classrooms, and personal book collections often rely on manual methods — spreadsheets, notebooks, or memory — to track which books are available and which have been borrowed. This makes it easy to lose track of inventory, difficult to quickly search for a specific title or author, and cumbersome to update a book's status when it's checked out or returned. There is a need for a lightweight, easy-to-use tool that lets a librarian or collection owner manage their catalog without the overhead of a full database system or graphical software.

## Scope of the Project

The Library Management System is a command-line application that allows a single user to manage a book inventory during a single running session. Its scope includes:

**In scope:**
- Viewing a formatted catalog of all books
- Searching the catalog by title or author
- Adding new books to the catalog
- Updating a book's status (Available / Checked Out)
- Removing books from the catalog
- Basic input validation to prevent crashes from invalid input

**Out of scope (for the current version):**
- Persistent storage (data is not saved between program runs)
- Multi-user access or simultaneous editing
- User authentication or accounts
- A graphical or web-based interface
- Due dates, fines, or borrower tracking
- Network or cloud functionality

This scope keeps the project focused on demonstrating core programming fundamentals — data structures, functions, and control flow — rather than production-level system design.

## Target Users

- **Beginner programmers / students** — using the project as a learning tool to understand functions, loops, and data structures in Python.
- **Small library or classroom managers** — who need a quick, no-install way to track a modest book collection without adopting complex library management software.
- **Personal book collectors** — who want a simple way to catalog and track their own books and lending status.

## High-Level Features

1. **Catalog Display** — View all books in a clean, structured table format (ID, Title, Author, Status).
2. **Search** — Look up books instantly by partial title or author name.
3. **Add Book** — Register new books into the catalog with title, author, and genre.
4. **Inventory Management** — Toggle a book's status between Available and Checked Out, or remove it from the catalog entirely.
5. **Robust Input Handling** — Prevents the program from crashing due to invalid menu choices or book IDs.
6. **Simple Menu-Driven Interface** — Easy navigation through numbered options, requiring no prior technical knowledge to use.
