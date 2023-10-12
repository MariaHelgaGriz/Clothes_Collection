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

ASSIGNMENT 3
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

ASSIGNMENT 4

What is UserCreationForm in Django? Explain its advantages and disadvantages.

The UserCreationForm in Django is a built-in form class provided by the Django system for the purpose of creating new user accounts. It is located within the 'django.contrib.auth.forms' module and is designed to streamline the creation of user registration forms in Django web applications. The advantages of utilizing the 'UserCreationForm' are its user-friendliness, offering pre-defined fields for common user registration details like username, email, and password, and its built-in validation checks, ensuring email uniqueness and password security compliance. Additionally, the form fields are easily customizable, and once a user registers, they can promptly log in, with their information securely stored in the database. However, there are certain disadvantages, including the form's inability to cover all registration data, necessitating the creation of custom forms for additional information, which may require a deeper understanding of Django's forms framework. Additionally, achieving a customized user interface may require additional CSS and templates. Lastly, it lacks built-in email verification functionality, necessitating the manual implementation of this feature.

What is the difference between authentication and authorization in a Django application? Why are both important?

Authentication and authorization serve distinct purposes in a Django application. Authentication validates a user's identity, while authorization determines the actions and resources an authenticated user can access and manipulate. These two components are essential because they collaborate to establish a secure and controlled user environment. Authentication prevents unauthorized access to the application, and authorization safeguards data and privacy. In a well-designed Django application, the synergy between these elements ensures both user authentication and controlled access, fostering data security and privacy.


What are cookies in website? How does Django use cookies to manage user session data?

Cookies are small data pieces sent by websites to users' web browsers and saved on their devices to record interactions. In Django, when a user accesses a site, a unique ID is created for them through the built-in framework. This framework also employs cookies to hold session data on the user's device, enhancing security by serializing and encrypting the information. Additionally, Django provides the option to store data securely on the server, allowing for greater security and larger storage capacity. It offers session data expiration settings to ensure validity. Furthermore, developers can customize it, specifying the data to store. It also implements CSRF protection by sending tokens with submissions to prevent unauthorized requests.

Are cookies secure to use? Is there potential risk to be aware of?

Correctly used, cookies are generally safe, but potential risks include data privacy concerns when sensitive information is stored without encryption, leaving it vulnerable to unauthorized access. Session hijacking is another risk, particularly if session IDs in cookies are inadequately managed. CSRF attacks are a concern when users are deceived into making malicious requests. Additionally, cookie theft can occur if attackers gain access to a user's device. Privacy concerns also arise when websites collect data through cookies without user consent. These risks can be mitigated by employing HTTPS for data encryption and by educating users about cookie usage and their options.


Explain how you implemented the checklist above step-by-step (not just following the tutorial).

Tutorial: Implementing Registration, Login, and Logout Functions

Step 1: Implement Registration Functionality
1. Use Django's built-in UserCreationForm to create a user registration form.
2. Set up a view (e.g., register) to handle user registration requests.
3. Process the form submission in the view, validate user input, and create a new user account using the form data.
4. Redirect the user to a login page or the main application page after successful registration.

   
Step 2: Implement Login Functionality
- Create a login form for users to enter their credentials (username and password).
- Set up a view (e.g., login_user) to handle user login requests.
- Authenticate the user using authenticate(request, username=username, password=password).
- If authentication is successful, log the user in using login(request, user).
- Redirect the user to the main application page upon successful login.

Step 3: Implement Logout Functionality
- Create a view (e.g., logout_user) to handle user logout requests.
- Use Django's logout(request) to log the user out and delete their session data.
- Redirect the user to the login page or another appropriate page after logging out.

Step 4: Create User Accounts with Dummy Data
- Register two user accounts using the registration form.
- For each user account, create three dummy data entries using the application's model (e.g., Item model).

Step 5: Connect Item Model with User
- Modify the Item model to include a foreign key field (e.g., user) that associates each item with a specific user.
- Ensure that each item is linked to the user who created it.

Step 6: Display Logged-In User Information
- In the main application page's template (e.g., main.html), retrieve and display information about the logged-in user.
- Display the username of the logged-in user (e.g., request.user.username).

Step 7: Apply Cookies for Last Login
- In the login_user view, create a response object using HttpResponseRedirect and set a cookie (e.g., "last_login") with the current date and time using response.set_cookie('last_login', str(datetime.datetime.now())).
- Display the "last_login" cookie data on the main application page (main.html) to show the user's last login time.

ASSIGNMENT 5

Explain the purpose of some CSS element selector and when to use it.

Applying particular HTML elements to a web page is what CSS element selectors are used for. Assuring an aesthetically pleasing and well-organized web design, they manage the presentation and layout of a web page's content using things like the tag name and a specific class attribute for numerous elements based on their relationship and properties.


Explain some of the HTML5 tags that you know.

Many semantic elements added by HTML5 improved the structure and organization of online pages. The terms "nav" and "article" designate areas for self-contained content, such as blog entries, respectively. "Footer" refers to a section of a page's footer, and "header" designates a header area frequently holding a page title or logo. Content is divided into several sections using the section> tag to facilitate better organization, accessibility, and SEO. These components facilitate the creation of well-organized, semantically relevant HTML documents by web developers, improving both their readability and visitors' user experiences.



What are the differences between margin and padding?

For spacing in web design, CSS features like margin and padding are employed. Padding is the area inside an element's border that creates space between the element's content and its border, whereas margin is the area outside an element's border that separates the element from its surroundings. Padding has an impact on the spacing and appearance of an element's content, whereas margins have an impact on the positioning and layout of elements on a page. For web development to produce the required style and visual design, it is essential to comprehend the distinction between margin and padding.

What are the differences between the CSS framework Tailwind and Bootstrap? When should we use Bootstrap rather than Tailwind, and vice versa?

Bootstrap and Tailwind CSS are CSS frameworks with different philosophies: With its granular control and strong customizability, Tailwind adheres to a utility-first philosophy and is perfect for applications needing distinctive designs and reduced file sizes. Contrarily, Bootstrap adopts a component-based methodology, making it perfect for projects looking for standardized, pre-designed UI components and for rapid prototyping. The decision between them depends on the requirements of your project and your preference for customisation against ease, with Bootstrap enabling speedy development with pre-made components and Tailwind excelling in precise styling. Some designers even blend the two for a well-rounded strategy.

The provided tutorial outlines several steps for enhancing a Django web application using the Bootstrap framework, adding a navigation bar, implementing an edit function, and adding a delete function. Here's a summarized breakdown of these steps:

Adding Bootstrap and JavaScript:
Open the base.html file in the templates folder of your Django project.
Inside the <head> section, add the <meta name="viewport"> tag for responsiveness.
Include Bootstrap CSS by adding a <link> tag pointing to the Bootstrap CDN.
Include JavaScript libraries like jQuery and Bootstrap's JavaScript files by adding <script> tags.
Integrate Bootstrap into your Django project, enhance the user interface with a navigation bar, and implement edit and delete functionality for your products by adding internal CSS styling directly within your HTML template, you can use the <style> element in the <head> section or apply inline styles directly to specific HTML elements. 

1. Internal CSS using <style> element:
define your CSS styles within the <style> element in the <head> section of your HTML template. 
CSS rules are defined within the <style> element, and they apply to the specified HTML elements.
2. Inline CSS:
apply CSS styles directly to individual HTML elements using the style attribute. Here's an example:
CSS styles are applied directly to individual HTML elements using the style attribute.
While inline styles are useful for making quick, specific adjustments, using the <style> element for internal CSS is preferable when you want to apply consistent styles across multiple elements or when you have more complex CSS rules.

Adding Edit Function:
In the views.py file of your Django app, create a new function (e.g., edit_product) that accepts request and id parameters.
Fetch the product to edit based on the provided ID.
Create a form instance with the product data.

Check if the form is valid and if the request method is POST, then save the edited data and redirect to the home page.
Create an edit_product.html template with a form that displays the product data for editing.
Add a URL pattern for the edit_product function in urls.py.
In the main.html template, add a button or link to access the edit page for each product.

Adding Delete Function:
Create a new function (e.g., delete_product) in views.py that takes request and id parameters.
Retrieve the product to delete based on the provided ID and delete it.
Redirect to the main page after deleting the product.
Add a URL pattern for the delete_product function in urls.py.
In the main.html template, add a button or link to delete each product, linking to the delete_product URL.

Testing:
Run Django project using python manage.py runserver.
Access the application in a web browser.

ASSIGNMENT 6

Explain the difference between asynchronous programming and synchronous programming.

There are two different methods for controlling processes and tasks in a computer programme: synchronous programming and asynchronous programming. Tasks are carried out consecutively, one after the other, and in a blocking manner in synchronous programming. When dealing with time-consuming or I/O-bound processes, delays in performance are possible since each job must finish before the next one begins. Unlike rather than blocking the main thread, asynchronous programming enables processes to run simultaneously. It makes it possible for a programme to start performing one task before moving on to another one without stopping to wait for the first one to finish. As a result, tasks that require waiting for external resources, such network requests, file I/O, or user interactions, can become more responsive and effective. In asynchronous programming, callbacks, promises, or async/await are frequently used.


In the implementation of JavaScript and AJAX, there is an implemented paradigm called the event-driven programming paradigm. Explain what this paradigm means and give one example of its implementation in this assignment.

JavaScript and AJAX event-driven programming paradigm is an approach where user interactions and events, rather than a straight-forward operation series, control the program's flow. Events are handled by callbacks or event handlers, which control how the programme operates.  This paradigm is used, for instance, in the assignment to manage a button click event, which causes a preset function to be called when the user hits the button. Due to their ability to respond to user activities without interfering with the main programme flow, this method makes web applications responsive and engaging. A fundamental idea in web development is event-driven programming, which enables programmers to make dynamic and user-friendly programmes by reacting to various user-initiated events like clicks, keypresses, or data retrieval.

Event Listeners: To react to user activities, event listeners are attached to a variety of HTML components, such as buttons and form inputs. As an illustration, the "Add Product by AJAX" button has an event listener that, when pressed, calls the addProduct method.

Asynchronous Event Handling: JavaScript functions like addProduct and refreshProducts handle events asynchronously. For example, when the "Add Product" button is clicked, the addProduct function is called, which uses the fetch API to send a POST request to add a product to the database without blocking the main thread.

Explain the implementation of asynchronous programming in AJAX.

The event-driven nature of JavaScript is used to implement asynchronous programming in AJAX, also known as Asynchronous JavaScript and XML, to carry out non-blocking activities. An AJAX request causes a web page to continue running other code rather than waiting for the response. This is accomplished using tools that allow the beginning of HTTP requests to a server, such as the XMLHttpRequest object or the fetch API. In order to handle multiple request phases, such as success or error, callback functions are given. Alternatives to using Promises or async/await to manage asynchronous actions more neatly and sequentially include the usage of contemporary JavaScript. By utilizing this strategy, web apps are guaranteed to be responsive and capable of rapidly completing activities, such as obtaining data from a server, without experiencing delays or obstructing the user interface.
In this semester, the implementation of AJAX is done using the Fetch API rather than the jQuery library. Compare the two technologies and write down your opinion which technology is better to use.

The requirements and context of the project strongly affect whether to use jQuery or the Fetch API to implement AJAX. Due to its native support for contemporary browsers, compatibility with contemporary JavaScript techniques, and lightweight design, the Fetch API is preferred for modern online applications. When browser compatibility is unimportant, it is a good option. On the other hand, developers who like a streamlined and user-friendly syntax and projects that need to support older browsers will find value in jQuery. Additionally, jQuery provides a wider range of tools for various web development jobs. jQuery is still relevant and useful for projects with historical requirements or where a more easy method is needed, however the Fetch API is advised for new projects targeting current browsers.

Step 1: Implementing a Function to Return Data as JSON
Create a new function in views.py called get_product_json that accepts a request as a parameter.
In the function, query the Product model and return the data as JSON using Django's serializers.serialize.
Set up the URL routing for get_product_json.

Step 2: Implementing a Function to Add Product using AJAX
Create a new function in views.py called add_product_ajax that accepts a request as a parameter.
Import csrf_exempt from django.views.decorators.csrf and apply it as a decorator above the add_product_ajax function to exempt it from CSRF protection.
In the add_product_ajax function, check if the request method is POST and extract data from the request.
Create a new Product object with the extracted data and save it to the database.
Return an HTTP response with a "CREATED" status if the product is successfully added.

Step 3: Add Routings for the get_product_json and add_product_ajax
Open urls.py and import the get_product_json and add_product_ajax functions.
Add URL paths for both functions inside the urlpatterns list.

Step 4: Showing the Product Data using the fetch() API
Open main.html and delete the table code created in a previous tutorial.
Add a <table> structure with the ID "product_table."
Create JavaScript functions getProducts and refreshProducts to fetch and display product data using the fetch() API.
Call the refreshProducts function to populate the table with data when the web page is opened.

Step 5: Creating a Modal as a Form to Add Products
Implement a form modal using Bootstrap in the app. The form collects data for adding new products.
This form includes fields for name, price, and description.

Step 6: Using AJAX to Add a Product
Create a JavaScript function called addProduct to add a new product using data from the modal form.
Use the fetch() API to send a POST request to the add_product_ajax view, including the form data as the request body.
After a product is added, call the refreshProducts function to update the product list in the table.
Reset the form fields after submission.
Set the addProduct function as the onclick handler for the "Add Product" button in the modal.










