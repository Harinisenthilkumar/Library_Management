📚 Library Management System
A comprehensive Library Management System developed to manage library operations such as tracking books, managing members, and handling book transactions like issues and returns. This system also integrates with the Frappe Library API for seamless data import.


🚀 Features
Books Management
Add, update, delete, and view book details.
Track book availability and stock.
Members Management
Maintain records of library members.
Manage member details and outstanding debts.
Transactions Management
Issue books to members.
Record the return of books.
Calculate and charge rental fees based on book return time.
Ensure that a member's outstanding debt does not exceed Rs. 500.
🔄 Use Cases
Perform CRUD operations on books and members.
Issue books to members and track book returns.
Search for books by title or author.
Automatically charge rental fees on book returns.
🔗 Frappe Library API Integration
To simplify adding new books to the system, the Frappe Library API has been integrated to allow for seamless book data imports:

API Endpoint:
https://frappe.io/api/method/frappe-library

Parameters:

page: to specify the page of the result set (for pagination).
title: to search for a specific book by title.
Example API Call:

bash
Copy code
curl https://frappe.io/api/method/frappe-library?page=2&title=and
Response Example:

json
Copy code
{
  "message": [
    {
      "bookID": "35460",
      "title": "Star Wars: Clone Wars Adventures Volume 6",
      "authors": "Haden Blackman",
      "publisher": "Dark Horse",
      "pageCount": 80
    }
  ]
}
This integration allows the system to import book data from external sources with minimal manual input, enhancing scalability and ease of use.

🛠️ Technologies Used
Backend: Python, Django
Frontend: HTML, CSS, JavaScript
Database: MySQL
API: Frappe Library API for book data imports
🗂️ Project Structure
bash
Copy code

📦 Library Management System
├── 📁 books
│   ├── 📄 models.py        # Book model definitions
│   ├── 📄 views.py         # CRUD operations for books
│   └── 📄 templates
│       └── 📄 book_list.html   # Template to display book data
├── 📁 members
│   ├── 📄 models.py        # Member model definitions
│   ├── 📄 views.py         # CRUD operations for members
│   └── 📄 templates
│       └── 📄 member_list.html   # Template to display member data
├── 📁 transactions
│   ├── 📄 views.py         # Handles book issues and returns
│   ├── 📄 models.py        # Tracks transactions and rental fees
├── 📄 requirements.txt      # Python dependencies
├── 📄 README.md             # Project documentation
└── 📄 manage.py             # Django management file
🔧 Installation & Setup

Clone the repository:
bash
Copy code
git clone https:https://github.com/Harinisenthilkumar/Library_Management
cd library-management-system
Install the dependencies:

bash
Copy code
pip install -r requirements.txt
Run migrations to set up the database:

bash
Copy code
python manage.py migrate
Start the development server:

bash
Copy code
python manage.py runserver
Access the system at http://127.0.0.1:8000/.

🌐 API Usage
You can import books into the system using the Frappe Library API as described in the "Frappe Library API Integration" section.


🤝 Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

Fork the repository.
Create a new feature branch.
Make your changes.
Open a pull request.
📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

