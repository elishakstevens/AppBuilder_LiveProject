# Live Project: My Korean Recipes
## Introduction
In this live project, I spent two weeks working with my peers on developing apps that track anything from sport stats to grocery costs using a database. I decided to track Korean Recipes, since I know Korean cuisine the best. I've always been very good at problem-solving and time management, and this live project really helped me apply those skills to software developement like I've never done before. I understand how to create a good quality product, and the work that goes into it. I was able to utilize important aspects of being a software developer within a real project, including Version Control, Project Management and Azure DevOps.  

The website is built with the Django framework, and I developed front-end and back-end in order to create a functioning app with a tracking database and form that displays beautifully on a screen.

## Back-End Development
Python was used to develop the back-end of my Korean Recipe App. Since the website uses Django as its framework, we need to configure this app in the apps.py in order for the app to function within this project.

![apps_KoreanFood](https://github.com/user-attachments/assets/bbd9b1e0-f375-4ec2-b049-5168ce84e85e)

In order for the website to connect to the app, I updated AppBuilder's settings.py and urls.py.

![setting_KoreanFood](https://github.com/user-attachments/assets/738e8863-e361-47c3-90ba-2f076f26b63b) ![url3_KoreanRecipe](https://github.com/user-attachments/assets/448d74d5-300a-40d3-be78-69718ba9c299)

I created a recipe model with properties that will be used to create a form and tracked through a database. When this class is referenced, it will return the dish name instead of the primary key.

![models_KoreanRecipes](https://github.com/user-attachments/assets/6a9914c9-a151-42ac-9822-ba6d6a4cda6d)

Once created, I registered this model in admin, creating the database.

![admin_KoreanRecipes](https://github.com/user-attachments/assets/50bf80cb-3ea5-442b-bd24-c41f8ee2ec02)

In order to view the home page and admin page, urls are created for each.

![url1_KoreanRecipes](https://github.com/user-attachments/assets/09f89f60-f197-4238-a741-b52db751e62c)

In order to add more recipes to the database, I created a form that any user can submit information through. On the back-end for this form, the Recipe model is used to inform the widgets that define each input and apply attributes to them for an easy to use form.

![form_KoreanRecipes](https://github.com/user-attachments/assets/ac40a421-0203-4219-8b32-5ef6abb276a5)

Now that I have a form (more on this in Front-End Development), the ability to add to the database and display the recipes for the user are added to views. We start views.py by rendering the home page. I also rendered a featured recipe page.

![view1_KoreanRecipe](https://github.com/user-attachments/assets/df938e51-7473-46ea-b7b5-8a510d15e676)

After this, I added a function that will save a new recipe if the form is filled in. Once saved, the user is redirected back to the home page. If not filled in, the function will render a blank form webpage.

![views2_KoreanRecipe](https://github.com/user-attachments/assets/4bce8afe-5e6c-424b-ab9b-2e8cffb31ab7)

I also wanted to be able to display all the recipes, as well as all the details about them. Both pages are rendered in views.py, where all the recipes are listed on one page, and when you click them, you are directed to that recipe's detail page. The primary key is used to connect a recipe in the database to the rendered details page.

![view3_KoreanRecipes](https://github.com/user-attachments/assets/dfd48b05-8b02-4cc9-81e7-399b02dc9693)

Along with these views, urls are needed in order to access them. The rest of the pages are added to urls.py. The details url includes the primary key of that recipe.

![url2_KoreanRecipe](https://github.com/user-attachments/assets/4c29495c-7e11-4f7c-a336-f4399b1e9490)


## Front-End Development
HTML, CSS, and Bootstrap were all used to display the form and the database that are easy for a user to use and view.

Every URL that I created in urls.py has a corresponding HTML page that is rendered through views.py, but to start, base.html is created. This contains the navigation bar and footer that will be on every webpage and extended via Jinja syntax.

![base1_KoreanRecipe](https://github.com/user-attachments/assets/2555cf43-0e4b-438e-8088-764522f62b1f)
![base2_KoreanRecipe](https://github.com/user-attachments/assets/0d24caa6-ffcf-4a2c-856d-b69c76697f8a)

External CSS and Bootstrap are linked here as well, which is used to style all of the app's webpages. All of the CSS is shown below.

![css_KoreanRecipe](https://github.com/user-attachments/assets/c041c41d-c4db-47ca-ad48-ca28f83d156f)
![css2_KoreanRecipe](https://github.com/user-attachments/assets/e4c0f60f-5912-46d9-8b95-16760c0a59a1)
![css3_KoreanRecipe](https://github.com/user-attachments/assets/e334e2d3-acac-4257-aee4-586cb0b69f49)

The app's homepage is created under index.html, which welcomes the user and includes a button that will take the user to the featured recipe.

![index_KoreanRecipe](https://github.com/user-attachments/assets/104beeb5-a6e4-46a2-b43d-cab9c1c4461b)

The featured page showcases my favorite recipe, tteokbokki!

![featured_KoreanRecipes](https://github.com/user-attachments/assets/cd1bd54a-3f71-4ad9-825e-ca33b8b89f49)

In order to allow the user to add another recipe, I created a webpage that displays a form with labels that are the paragraph 'p' tag font size and a submit button.

![add_KoreanRecipes](https://github.com/user-attachments/assets/9d9d3f0f-5cc3-4dac-9817-98d533d76fcc)

With this recipes database, I can pull entries and display them how I want. I pull all of the current recipes and display the dish names on a webpage where each name is linked to that recipe's details page. 

![all_KoreanRecipes](https://github.com/user-attachments/assets/61684ba8-20fe-4a92-813c-ca651ebcbb29)

Each detail page is the entire selected recipe. This one page uses Jinja syntax to pull the recipe information from the details function in views.py in order to display any recipe that is selected.

![details_KoreanRecipes](https://github.com/user-attachments/assets/901075ff-cc30-45f2-ba5d-77454d0d92af)

## Other Skills
- Identifying bugs in my own code and repairing them
- Problem-solving how to code certain elements or functions in the most efficient way that works with the rest of the project
- Scheduling work and managing time in order to make project deadlines
