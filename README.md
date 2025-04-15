# My Blog
Vinay's Blog
A simple Django blog application where users can view a list of posts and click to read full content.

Project Overview
This is a basic blog application built with Django. It displays blog posts on the homepage and provides a detailed view of each post when clicked.

Key Features:
Homepage: Displays a list of all blog posts with a preview.

Detailed Post View: Clicking on a post redirects to a page displaying the full content of that post.

Responsive Design: Adjusts the layout for mobile and desktop views.

How It Works
Models:

The blog uses a Post model with the following fields:

title: The title of the post.

body: The content of the post.

created_at: Timestamp when the post is created.

Views:

index: Fetches all blog posts from the database and passes them to the homepage template (index.html).

post: Fetches a single post by its ID (primary key) and renders the detailed post template (post.html).

URLs:

The project defines two main routes in urls.py:

/: Displays all posts using the index view.

/post/<str:pk>: Displays a single post based on its ID.

Templates:

index.html: Displays a list of posts with the title, creation date, and a truncated preview of the body.

post.html: Displays the full content of a specific post when clicked.

Tech Stack
Backend: Django (Python framework)

Frontend: HTML + CSS

Database: SQLite (default database in Django)

Version Control: Git for version management

Setup and Installation
Prerequisites:
Python 3.x installed on your system

Django 3.x or above installed

Installation:
Clone the repository:

bash
Copy
Edit
git clone <repository_url>
Navigate to the project folder:

bash
Copy
Edit
cd <project_name>
Create a virtual environment:

nginx
Copy
Edit
python3 -m venv venv
Activate the virtual environment:

For Windows:

Copy
Edit
venv\Scripts\activate
For macOS/Linux:

bash
Copy
Edit
source venv/bin/activate
Install dependencies:

nginx
Copy
Edit
pip install -r requirements.txt
Apply migrations:

nginx
Copy
Edit
python manage.py migrate
Run the server:

nginx
Copy
Edit
python manage.py runserver
Visit http://127.0.0.1:8000/ in your browser to view the blog.

Future Enhancements
Add user authentication to allow users to log in and create posts.

Implement comments on posts.

Add tags to categorize posts.

Include a search feature to find posts.

License
This project is licensed under the MIT License – see the LICENSE file for details.
