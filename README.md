# Clothes_Collection
How do you implement the tasks in the checklist? Explain in a step-by-step manner (not just copy-paste from the tutorial).
Step-by-step setting up a Django project and using its essential parts:

1. Create a Django project by using the django-admin startproject projectname command.
- Use the command cd projectname to go to the project directory.
2. Define a Data Model
- Use Django's ORM to define the data model in your app's models.py file.
3. Generate database migrations
- Using Python manage.py makemigrations, create basic database migrations.
- Utilize Python manage.py migrate to apply migrations to build the database schema.
4. Make a View:
- To handle HTTP requests and responses, define views in views.py.
5. Map URL Patterns to View Functions:
- Using Django's URL Patterns, define URL patterns to map to view functions in your app's urls.py file.
6.Create HTML Templates: 
- In the templates folder of your app directory, design and produce HTML templates.
7.Use Django Template Language:
- To display data from views, use HTML templates that are written in Django Template Language.
8. Setting up the project:
- Add your app to the INSTALLED_APPS list in settings.py.
- To provide the template directory, configure the TEMPLATES option.
9.Develop Server to run:
- Python manage.py runserver can be used to launch the development server.
- Use the supplied URL to access your app, such as http://127.0.0.1:8000.
10. Test Your Program:
- Create test data for your model using either the admin interface or scripts.
- To test how templates present data, access URLs connected to views.
11. Optional Deployment:
- If necessary, use hosting providers like Adaptable.io to deploy your Django application into production. adhere to their deployment instructions.
- These steps will help to establish a working Django web application that includes models, views, templates, and URLs.

Create a diagram explaining the flow of client requests to a Django web app and its response. Also in the diagram, explain the connections between urls.py, views.py, models.py, and the HTML file(s).


![Assignment1_MariaHelgaGrizelda_2206046733 drawio](https://github.com/MariaHelgaGriz/Clothes_Collection/assets/134635504/56558884-9004-4f57-a02f-f4d99883537e)

What is the purpose of a virtual environment? Can we create a Django web app without a virtual environment?


By offering a variety of highlights, a virtual environment acts as a significant tool in Python development. As a result, each project can run independently with its own libraries and dependencies thanks to the ability to create isolated environments for distinct projects. Along with preventing conflicts between projects, this isolation also provides fine-grained control over package management, allowing the installation, updating, and removal of project-specific packages without affecting the Python installation across the entire system. Virtual environments also make collaboration and code sharing easier by enabling version control of project dependencies. By making environments more portable, they make it possible for programmers to recreate reliable development environments on many devices. Finally, virtual environments improve security by reducing the risks brought on by system-wide package conflicts by isolating project dependencies.
Finally, to answer the second queston, yes it is technically possible to create a Django Web app without a virtual environment, but managing dependencies and version control could be problematic, making it challenging to share and maintain your project. 

What is MVC, MVT, and MVVM? Explain the differences between the three.


Software applications are organized using the architectural patterns MVC, MVT, and MVVM, which define specific roles for components. In MVC, the Controller is in charge of user input and flow control, the View is in charge of presentation, and the Model is responsible for data and business logic. MVT, as used in Django, is similar to MVC but provides a Template to customize the user interface and permits some control logic in the View. The ViewModel acts as a go-between for the Model and View in MVVM, which emphasizes a more adaptable and reactive approach. It performs exceptionally well with data-binding frameworks like Angular and Vue. In conclusion, MVVM enables improved separation of concerns, particularly in modern front-end development, enabling fast data processing and presentation. MVC and MVT both have their place in standard and web applications.

ASSIGNMENT 2
What is the difference between POST form and GET form in Django? in one paragraph

The main difference between POST and GET forms in Django is how they manage form data submission. Using a POST form increases security because the form data is not exposed in the URL and is transmitted in the request body, making it appropriate for sensitive or massive data such as login credentials or file uploads. In contrast, a GET form adds form data to the URL as query parameters, making it appropriate for straightforward data retrieval or search queries, but the data is visible in the URL, which may not be the best option for sensitive information.

What are the main differences between XML, JSON, and HTML in the context of data delivery? in one paragraph

Data transmission uses XML (Extensible Markup Language), JSON (JavaScript Object Notation), and HTML for various applications. HTML is used to specify the structure and layout of web documents, primarily for presentation in web browsers, while XML is a detailed and hierarchical markup language used primarily for structuring and storing data. JSON is a lightweight, key-value pair-based format that is popular for efficient and human-readable data interchange, particularly in modern web applications. JSON excels in simplicity and efficiency, whereas XML offers stringent data validation, and HTML concentrates on generating material for web consumption. Each format has its advantages and applications.

Why is JSON often used in data exchange between modern web applications? in one paragraph

JSON (JavaScript Object Notation) is frequently utilised in data transmission across current online applications. It is straightforward to write, human-readable, and lightweight, which makes it effective for data transmission over networks and facilitates development and debugging. JSON is a flexible option for data exchange in heterogeneous situations because it is language-agnostic, or supported by a wide range of computer languages. Additionally, JSON is extensively supported in APIs and web services, making it a common alternative for data transmission and facilitating easy integration between various systems and applications. It can also be swiftly parsed in modern web browsers and server-side technologies, improving performance.

Explain how you implemented the checklist above step-by-step (not just following the tutorial).

Step 1: Create a Model Form for Input

In Django app's folder (e.g., main), open or create a file named forms.py if it doesn't exist.
Define a form class that inherits from ModelForm. Replace YourModel with the actual model you want to create objects for, and specify the fields you want to include in the form.

Step 2: Create Five Views to Display Model Objects

Open app's views.py file.
Create five views, each responsible for displaying model objects in different formats.

Step 3: Set Up URL Routing for Views

In app's urls.py file, import the views created.
Define URL patterns for each view using Django's path or re_path function.









