# Financial Toolkit in Python (Beginner Level)

This project implements a mini financial system divided into three main modules:
  1. Investment calculator (compound interest)
  2. Portfolio evaluator (weights and dominant asset)
  3. Wallet / Expense tracker (income, categories, ranking, category sets)

Everything is developed using only basic Python, with:
  • functions  
  • input validation  
  • lists  
  • dictionaries  
  • tuples  
  • sets  
  • loops and conditionals  
  • interactive menus  

It does not depend on external files, additional libraries, or document read/write operations.

---

## Main Features

### 1) Investment Calculator

Calculates the final return of an investment using the compound interest formula:

C_n = C_0 (1 + r)^n

Includes:
  • initial capital  
  • annual rate (in %)  
  • number of years  
  • automatic calculation of the final amount  
  • optional year-by-year growth table  

---

### 2) Portfolio Evaluator

Allows registering assets with their ticker and invested amount.  
Calculates:
  • Total invested  
  • Percentage weight of each asset  
  • Asset with the highest weight  

Example input:

AAPL: $3000
TSLA: $1500
VOO:  $550

Example output:

Total: 10,000 MXN
AAPL → 30%
TSLA → 15%
VOO → 55%  ← mayor peso

### 3) Wallet and Expense Evaluator

Interactive system to record:

INGRESO, OTROS, 8000
GASTO, COMIDA, 300
GASTO, TRANSPORTE, 200
GASTO, ENTRETENIMIENTO, 1500

Includes:
  • List of transactions (list of dictionaries)  
  • Classification by categories using dictionaries  
  • Validation with tuples  

TIPOS_VALIDOS = ("INGRESO", "GASTO")
CATEGORIAS_VALIDAS = ("COMIDA", "ENTRETENIMIENTO", ...)

  • Unique categories used (set)  
  • Categories with high expenses (>1000) (set)  
  • Expense ranking sorted from highest to lowest  

Example output:

Saldo total: 7200.00
Categorías usadas: COMIDA, TRANSPORTE, ENTRETENIMIENTO, OTROS
Categorías de gasto alto (>1000): ENTRETENIMIENTO
Ranking:
1. ENTRETENIMIENTO - 1500
2. SERVICIOS - 800
3. COMIDA - 300

## Project Structure

The program is organized into modules:

'''
FinancialToolkit.ipynb  
├── secure input handlers  
├── Section A  
│   ├── investment calculator  
│   └── portfolio evaluator  
├── Section B  
│   └── wallet and expense analyzer  
└── main (main menu and flow)
'''

The notebook contains 5 cells in total:  
  1. Input validation functions  
  2. Investment calculator  
  3. Portfolio evaluator  
  4. Wallet  
  5. Main menu and execution  


## Author

Project developed by Jorge Daniel Gómez Quintana  
Degree: Data Science and Artificial Intelligence – ITAM  
