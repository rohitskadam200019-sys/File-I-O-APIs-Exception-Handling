# Python API & Error Logging Project (Part 3)

This repository contains the final submission for the Python Programming Assignment, focusing on advanced API interactions, file management, and robust error handling.

## Project Structure

* **`part3_api_files.ipynb`**: The main Google Colab notebook containing all Python logic and task solutions.
* **`python_notes.txt`**: A generated summary of key Python concepts including variables, lists, and modules.
* **`error_log.txt`**: A persistent log file that records network errors and HTTP failures with precise timestamps.

## 🛠️ Key Features

### 1. Robust API Integration
Implemented a safe API fetcher using the `requests` library that handles:
* **Connection Errors**: Catches network-level failures.
* **Timeouts**: Prevents the script from hanging by using a 5-second limit.
* **Status Code Validation**: Specifically identifies 404 "Not Found" responses vs. successful 200 responses.

### 2. Automated Error Logging
A custom logging function was built to:
* Use the `datetime` module for real-time timestamps.
* Operate in **Append Mode (`'a'`)** to ensure log history is preserved across multiple runs.
* Log both Python exceptions and manual HTTP error checks.

### 3. Input Validation Loop
The interactive product lookup tool ensures that only valid integers between 1 and 100 are processed, preventing unnecessary or broken API calls.

## 🚀 How to Run
1. Open the `.ipynb` file in Google Colab or Jupyter Notebook.
2. Run the cells in order.
3. When prompted, enter a Product ID (1-100) or type 'quit' to finish.
4. Check the local directory for the generated `.txt` files to view the output logs.
