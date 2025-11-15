# Sudoku Application Setup Guide

## Image Resources

The application expects image files in a `resources/` directory. Please create this directory and add the following image files:

```
resources/
├── question.png      (Question mark icon for help buttons)
├── checked.png       (Checkmark icon for verification)
├── file.png          (File icon for the application)
├── sudoku.png        (Sudoku icon for the main game window)
├── back.png          (Back button icon)
└── check.png         (Check/success icon)
```

## Directory Structure

```
Sudoku-Using-Backtracking/
├── Driver.java
├── Sudoku.java
├── README.md
├── SETUP.md (this file)
└── resources/
    └── (image files)
```

## Note

If image files are not found, the application will use transparent fallback images and continue running without crashing. Warnings will be printed to the console for any missing images.

## Compilation

This is a JavaFX application. To compile and run:

1. Ensure JavaFX SDK is installed and configured
2. Compile: `javac --module-path /path/to/javafx-sdk/lib --add-modules javafx.controls,javafx.fxml Driver.java Sudoku.java`
3. Run: `java --module-path /path/to/javafx-sdk/lib --add-modules javafx.controls,javafx.fxml com.example.demo29.Driver`

## Changes Made

- Removed hard-coded absolute Windows file paths (e.g., `C:\\Users\\issam\\Downloads\\...`)
- Implemented safe image loading with fallback mechanism
- Made the application portable across different operating systems and user environments
