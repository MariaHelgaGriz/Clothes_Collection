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
- If necessary, use hosting providers like Heroku, AWS, or DigitalOcean to deploy your Django application into production. adhere to their deployment instructions.
- These steps will help to establish a working Django web application that includes models, views, templates, and URLs.

Create a diagram explaining the flow of client requests to a Django web app and its response. Also in the diagram, explain the connections between urls.py, views.py, models.py, and the HTML file(s).


![Assignment1_MariaHelgaGrizelda_2206046733 drawio](https://github.com/MariaHelgaGriz/Clothes_Collection/assets/134635504/56558884-9004-4f57-a02f-f4d99883537e)

What is the purpose of a virtual environment? Can we create a Django web app without a virtual environment?


By offering a variety of highlights, a virtual environment acts as a significant tool in Python development. As a result, each project can run independently with its own libraries and dependencies thanks to the ability to create isolated environments for distinct projects. Along with preventing conflicts between projects, this isolation also provides fine-grained control over package management, allowing the installation, updating, and removal of project-specific packages without affecting the Python installation across the entire system. Virtual environments also make collaboration and code sharing easier by enabling version control of project dependencies. By making environments more portable, they make it possible for programmers to recreate reliable development environments on many devices. Finally, virtual environments improve security by reducing the risks brought on by system-wide package conflicts by isolating project dependencies.
Finally, to answer the second queston, yes it is technically possible to create a Django Web app without a virtual environment, but managing dependencies and version control could be problematic, making it challenging to share and maintain your project. 

What is MVC, MVT, and MVVM? Explain the differences between the three.


Software applications are organized using the architectural patterns MVC, MVT, and MVVM, which define specific roles for components. In MVC, the Controller is in charge of user input and flow control, the View is in charge of presentation, and the Model is responsible for data and business logic. MVT, as used in Django, is similar to MVC but provides a Template to customize the user interface and permits some control logic in the View. The ViewModel acts as a go-between for the Model and View in MVVM, which emphasizes a more adaptable and reactive approach. It performs exceptionally well with data-binding frameworks like Angular and Vue. In conclusion, MVVM enables improved separation of concerns, particularly in modern front-end development, enabling fast data processing and presentation. MVC and MVT both have their place in standard and web applications.

