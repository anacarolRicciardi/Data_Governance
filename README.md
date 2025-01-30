# PostgreSQL Data Governance and Privacy Techniques

This repository contains Jupyter notebooks that demonstrate various **data governance and privacy techniques** using **PostgreSQL**. The examples cover database management, user access control, pseudonymization, perturbation, suppression, and other privacy-preserving techniques.

## 📌 Notebooks Included

### 1️⃣ **PostgreSQL Data Governance - Auto DB Creation**
   - Automatically creates a PostgreSQL database if it does not exist.
   - Manages user roles and privileges.
   - Implements access control for a `patients` table.
   - Inserts sample data for testing security policies.

### 2️⃣ **PostgreSQL Data Governance - New Data**
   - Similar to the first notebook but with **different sample data**.
   - Useful for testing new security policies with varied datasets.

### 3️⃣ **PostgreSQL Pseudonymization**
   - Demonstrates pseudonymization techniques for sensitive data.
   - Uses hashing to anonymize patient names and countries.
   - Ensures compliance with privacy regulations while preserving usability.

### 4️⃣ **PostgreSQL Data Perturbation**
   - Introduces controlled noise into numerical fields (e.g., medical expenses).
   - Ensures that data remains statistically useful while preventing re-identification.
   - Useful for privacy-preserving analytics and research.

### 5️⃣ **PostgreSQL Data Suppression**
   - Suppresses financial data based on predefined thresholds.
   - Ensures that sensitive data is hidden while maintaining dataset integrity.
   - Helps enforce compliance with data privacy laws.

## 🚀 Getting Started

### Prerequisites
- Install PostgreSQL 13 or later
- Install Python 3.8 or later
- Required Python libraries:
  ```bash
  pip install sqlalchemy psycopg2 pandas
  ```

### Running the Notebooks
1. Start your PostgreSQL server and ensure it is accessible.
2. Open Jupyter Notebook or Jupyter Lab:
   ```bash
   jupyter notebook
   ```
3. Navigate to the desired notebook and execute the cells step by step.

## 🛠️ Configuration
If the database connection fails, verify your **PostgreSQL settings** in the notebook:
```python
PG_ADDR = 'localhost'  # PostgreSQL Server Address
PG_PORT = '5432'       # Default PostgreSQL Port
PG_USER = 'postgres'   # Admin User
PG_PASW = 'secure_password'  # Database Password
PG_DBNA = 'healthcare_db'  # Database Name
```
Modify these credentials based on your environment.

## 🔐 Privacy and Security Techniques
These notebooks simulate a **healthcare database**, ensuring:
- Secure access control for different roles (Nurses, Doctors, Consultants).
- Protection of patient records with pseudonymization, suppression, and perturbation.
- Compliance with **data privacy regulations**.

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing
Pull requests are welcome! If you find any issues or improvements, please submit an issue or PR.

## 📞 Contact
For any questions, feel free to reach out via GitHub Issues.

Happy coding! 🚀
