# Document Converter

A simple desktop application for converting PDF and image files into machine-readable `.docx` documents using Optical Character Recognition (OCR).

## Features

-   User-friendly graphical interface.
-   Supports PDF, PNG, JPG, BMP, and TIFF files.
-   Automatically detects if a PDF contains a text layer or requires OCR.
-   Saves converted documents as `.docx` files.
-   Allows users to configure a target directory for saved files.
-   Native look and feel on Windows.
-   Provides user feedback with "please wait" messages and error pop-ups.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

1.  **Python 3.6+**: You can download it from [python.org](https://www.python.org/downloads/).
2.  **Tesseract OCR Engine**: This is required for the OCR functionality.
    -   You can find installation instructions on the official [Tesseract documentation](https://tesseract-ocr.github.io/tessdoc/Installation.html).
    -   **Important**: After installing, you must add the Tesseract installation directory to your system's `PATH` environment variable.

## Setup & Installation

1.  **Clone the repository:**
    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```

2.  **Create a Python virtual environment (recommended):**
    ```bash
    # On Windows
    python -m venv venv
    venv\Scripts\activate

    # On macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

## Running the Application

Once the setup is complete, you can run the application with the following command:

```bash
python app.py
```

## How to Use

1.  **Set the Target Folder:**
    -   Before you can process any files, you must set a folder where the converted `.docx` files will be saved.
    -   Click on `File` -> `Set Target Folder` from the menu bar.
    -   Choose a directory from the dialog. Your selection will be saved for future sessions.

2.  **Upload and Convert Files:**
    -   Click the `Upload Files` button.
    -   Select one or more PDF or image files from the file dialog.
    -   The application will show a "Please wait..." message while it processes the files.
    -   Once complete, the converted `.docx` files will be available in the target folder you specified.
    -   You will receive a notification upon success or if any errors occurred.
