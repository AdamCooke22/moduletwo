# Loan Qualifier Application

This is a python command-line interface application that allows users to see qualifying loans from lenders quickly and easily. The application works by taking in a `daily_rate_sheet` of loan criteria from various loan providers, asking the user a number of questions to evaluate their loan eligibility, and then returning to them a list of qualifying loans.

---

## Technologies

This project leverages python 3.7 with the following packages:

* [fire](https://github.com/google/python-fire) - For the command line interface, help page, and entrypoint. Python Fire allows us to convert our Python code into a command-line interface very easily.

* [questionary](https://github.com/tmbo/questionary) - For interactive user prompts and dialogs. Questionary allows us to utilize input prompts to obtain necessary information from users.

---

## Installation Guide

Before running the application first install the following dependencies.

```python
  pip install fire
  pip install questionary
```

---

## Usage

To use the loan qualifier application simply clone the repository and run the **app.py** with:

```python
python app.py
```

Upon launching the loan qualifier application you will be greeted with the following prompts. The information that is inputed is used and filtered through certain criteria (For example credit score, debt to income, loan to value,max laon size) that automatically find the loans (if any) that match from data/daily_rate_sheet.csv If the user wishes to save the qualified loans to their computer, the program will prompt the user where on their computer they would like to save the CSV file.


If the information provided qualifies for a loan or more you will be granted with this prompt. ![loan_qualifier_app_qualified](https://user-images.githubusercontent.com/107158380/178882201-0e73ab29-b234-45c9-ae6d-86a5d1c0f134.png)


If the information provided does not qualify for any loans you will be granted with this prompt. ![loan_qualifier_app_not_qualified](https://user-images.githubusercontent.com/107158380/178882347-d5468b63-ede3-4421-b38c-8f5e09a49112.png)


## Documentation
To generate a text file of the command history, the code history 50 > terminal_history.txt is used to display the last 50 commands that were entered into the terminal. [terminal_history.txt](https://github.com/AdamCooke22/moduletwo/files/9107983/terminal_history.txt)


---

## Contributors

Completed by Adam Cooke

---

## License

MIT
