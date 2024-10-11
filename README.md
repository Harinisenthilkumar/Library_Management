📚 Library Management System
A comprehensive system developed to manage library operations such as tracking books, managing members, and handling book transactions like issues and returns. The system also calculates rental fees and tracks member debts to ensure smooth transactions.

🚀 Features
📖 Books Management:

Add, update, delete, and view book details.
Track book availability and stock.
👥 Members Management:

Maintain detailed records of library members.
Manage member debts and ensure outstanding amounts do not exceed Rs. 500.
🔄 Transactions Management:

Issue books to members and record book returns.
Calculate and charge rental fees based on the time of return.
🔄 Use Cases
Perform CRUD operations on books and members.
Issue and return books, tracking transactions.
Search books by title or author.
Automatically charge rental fees upon book return.
🛠️ Technologies Used
Backend: Python, Django
Frontend: HTML, CSS, JavaScript
Database: MySQL
🗂️ Project Structure
bash
Copy code
📦 Library Management System
├── 📁 books
│   ├── 📄 models.py        # Book model definitions
│   ├── 📄 views.py         # CRUD operations for books
│   └── 📁 templates
│       └── 📄 book_list.html   # Template to display book data
├── 📁 members
│   ├── 📄 models.py        # Member model definitions
│   ├── 📄 views.py         # CRUD operations for members
│   └── 📁 templates
│       └── 📄 member_list.html   # Template to display member data
├── 📁 transactions
│   ├── 📄 views.py         # Handles book issues and returns
│   ├── 📄 models.py        # Tracks transactions and rental fees
├── 📄 requirements.txt      # Python dependencies
├── 📄 README.md             # Project documentation
└── 📄 manage.py             # Django management file
🔧 Installation & Setup
1. Clone the repository:
bash
Copy code
git clone https://github.com/Harinisenthilkumar/Library_Management.git
cd library-management-system
2. Install the dependencies:
bash
Copy code
pip install -r requirements.txt
3. Run migrations to set up the database:
bash
Copy code
python manage.py migrate
4. Start the development server:
bash
Copy code
python manage.py runserver
📍Access the system at: http://127.0.0.1:8000/

🌐 API Integration (Optional)
You can integrate with the Frappe Library API to import books into the system.

📸 Screenshots
Here are some visual previews of the system:



🤝 Contributing
Contributions are welcome!
To contribute:

Fork the repository.
Create a new feature branch.
Make your changes.
Open a pull request.
📝 License
This project is licensed under the MIT License. See the LICENSE file for more details.

✨ Hope you find this project interesting! Feel free to connect and discuss improvements or extensions. Happy coding! 😊
