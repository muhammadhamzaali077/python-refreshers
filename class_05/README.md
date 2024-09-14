# Python Refreshers class_05

This repository provides a simple tutorial on using conditional statements in Python. The examples demonstrate how to use `if`, `elif`, and `else` statements for decision-making in various scenarios, such as checking eligibility, assigning grades, and verifying user bans.

## Overview

This project covers the following key concepts:
- Writing conditional statements using `if`, `elif`, and `else`
- Decision-making based on user input or variable conditions
- Implementing basic logic to handle different cases

## Requirements

To run the code in this project, you need:
- Python 3.12

## Code Examples

### Eligibility Check

This example checks if a customer is eligible for a CNIC based on their age.

```python
customers_name : str = "Hamza"
customer_age : int = 19

if customer_age == 18:
    print("You are eligible for CNIC")
else:
    print("You are not eligible for CNIC")
```

### Grade Assignment

This example determines a student's grade based on their percentage.

```python
percentage : float = 100

if percentage > 100:
    print("Invalid percentage")
elif percentage >= 80:
    print("Your Grade is A+")
elif percentage >= 70:
    print("Your Grade is A")
elif percentage >= 60:
    print("Your Grade is B")
elif percentage >= 50:
    print("Your Grade is C")
elif percentage >= 40:
    print("Your Grade is D")
else:
    print("Your Grade is F")
```

### Banned User Check

This example checks if a user is banned by comparing their username against a list of banned users.

```python
from typing import List

banned_users : List[str] = ["ali", "usama"]
user : str = "USAMA"
checking : bool = user.lower() in banned_users

if checking:
    print("You are banned")
else:
    print("You are not banned, you can go")
```

## Usage

To run the examples:
1. Clone the repository.
2. Open the `class_05.ipynb` notebook in your Jupyter environment.
3. Execute the cells to see the conditional logic in action.

## Setting Up Google Colab

Google Colab is a free platform for running Python code in the cloud. Follow these steps to set up and run the notebook on Colab:

### Steps to Set Up

1. Open [Google Colab](https://colab.research.google.com/).
2. If prompted, sign in with your Google account.
3. To upload the notebook:
   - Click on **File** > **Upload Notebook**.
   - Upload the `class_05.ipynb` notebook from your local machine.
4. Once the notebook is uploaded, you can start running each cell by clicking the "Run" button (play icon) on the left of each code cell.

### Features of Google Colab

Google Colab offers several advantages for Python programming:

- **Cloud-based**: No need to install Python or any libraries on your local machine.
- **Free GPU support**: You can access powerful hardware, including GPUs and TPUs, for free.
- **Collaborative**: Share your notebook with others and collaborate in real-time, similar to Google Docs.
- **Pre-installed libraries**: Many popular Python libraries, such as NumPy, pandas, and TensorFlow, are pre-installed.
- **Easy integration with Google Drive**: You can directly save and load files from Google Drive, making it easier to manage your data and projects.

To use Google Drive with Colab, you can mount it using the following code in your Colab notebook:

```python
from google.colab import drive
drive.mount('/content/drive')
```

This will allow you to access your Google Drive files from within the notebook.
