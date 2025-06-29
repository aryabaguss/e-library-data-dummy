# E-Library Data Dummy Generator

A Python-based dummy data generator for e-library application databases. This project creates realistic sample data for various e-library system tables, which can be exported as CSV files and imported into PostgreSQL databases using pgAdmin4.

## 📋 Overview

This project generates comprehensive dummy data for e-library systems including:
- User accounts
- Book catalog with detailed metadata
- Book categories and genres
- Borrowing transactions and history
- Reservation records
- Library branch information

## 🛠️ Technologies Used

- **Python 3.x** - Main programming language
- **Jupyter Notebook** - Development environment
- **Faker** - Primary library for generating realistic fake data
- **Pandas** - Data manipulation and DataFrame operations
- **NumPy** - Numerical operations and array handling
- **Random** - Additional randomization functions
- **Datetime** - Date and time operations


## 🚀 Getting Started

### Usage

1. **Run the notebook cells sequentially** to generate dummy data for different tables
2. **Configure data volume** by modifying the variables at the beginning of each section:
   ```python
   # Example: Generate 1000 users
   NUM_USERS = 1000
   NUM_BOOKS = 5000
   NUM_BORROWING_RECORDS = 2000
   ```

3. **Execute data generation** - Each section will create realistic data for specific tables

4. **Export to CSV** - The generated DataFrames are automatically exported to CSV files in the `output/` directory

5. **Import to PostgreSQL** - Use pgAdmin4 to import the generated CSV files into your database tables

## ⚙️ Customization
### Localization
Modify Faker locale for region-specific data:

```python
from faker import Faker
fake = Faker('id_ID')  # Indonesian locale
# or
fake = Faker(['en_US', 'id_ID'])  # Multiple locales
```

## 🔧 Troubleshooting

### Common Issues
**CSV encoding problems:**
- Specify UTF-8 encoding when exporting
- Check for special characters in generated data

**Database import errors:**
- Verify column data types match CSV data
- Check for null values in required fields
- Ensure foreign key relationships are valid

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Arya Bagus** - [aryabaguss](https://github.com/aryabaguss)

## 🙏 Acknowledgments

- [Faker](https://github.com/joke2k/faker) - For providing excellent fake data generation capabilities
- [Pandas](https://pandas.pydata.org/) - For powerful data manipulation tools
- PostgreSQL and pgAdmin4 communities for database management tools

