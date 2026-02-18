# PSUSphere

**PSUSphere** is a web app made with Django. It helps manage student organizations, colleges, programs, and memberships. It has a clear backend and a simple admin page for handling data.

## What It Does

This app is a central place to track student involvement in campus groups. It uses Django’s database system to connect:
- **Colleges** (like College of Sciences)  
- **Programs** (like BS Computer Science)  
- **Organizations** (like Association of Computing Students)  
- **Students** and their **Memberships**

Admins can add, edit, delete, and view records. They can also create fake data for testing.

## Features

- **Organization Management:** Connect organizations to their colleges.  
- **Student Records:** Store student info such as ID and program.  
- **Membership Tracking:** Record which students joined which groups and when.  
- **Admin Page Improvements:**  
  - **Search:** Find students, programs, or organizations fast.  
  - **Filters:** Narrow results by college or join date.  
  - **Custom Views:** Cleaner list displays.  
- **Data Automation:** A command (`create_initial_data`) makes fake data with the Faker library.

## Tech Used

- **Python** – backend code  
- **Django** – web framework  
- **SQLite** – database  
- **Faker** – fake data generator  

## Setup

1. **Clone the project:**

   >git clone https://github.com/yourusername/PSUSphere.git
   >cd PSUSphere

2. **Make and activate a virtual environment:**

    - Windows
    >python -m venv psusenv
    >psusenv\Scripts\activate

    - Mac/Linux
    >python3 -m venv psusenv
    >source psusenv/bin/activate

3. **Install requirements:**

    >pip install -r requirements.txt

4. **Apply database migrations:**
    
    >cd projectsite
    >python manage.py makemigrations
    >python manage.py migrate
    

5. **Create a superuser (Admin):**
    
    >python manage.py createsuperuser
    

6. **(Optional) Load initial data:**
    
    >python manage.py create_initial_data
    

7. **Run the server:**
    
    >python manage.py runserver
    

## Usage

1.  Open your browser and navigate to: http://127.0.0.1:8000/admin/
2.  Log in using the superuser credentials you created.
3.  Navigate through the *Studentorg* section to manage Colleges, Organizations, and Students.

## Authors

* *[Shena D. Pebula]* - Repository Owner
* *[Mary Dianne O. Millendez]* - Collaborator

---
Rev 01 - August 2025
github.com