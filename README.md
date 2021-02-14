# BiaBook

### [BiaBook Live Site](https://biablog.herokuapp.com//)

### [GitHub Repository](https://github.com/AlexNexton/biablog)

![Various Devices](https://github.com/Sean-Mc-Mahon/McTasticRecipes/blob/master/wireframes/resposiveness.JPG)

BiaBook (where 'bia' is the Irish word for food) is my Milestone 3 project.
It is part of the Fullstack Software Development Course of [Code Institute](https://codeinstitute.net/).

# Table of Contents

**<details><summary>Project overview</summary>**
* [**_Project overview_**](#project-overview)
* [**_User Stories_**](#user-stories)
* [**_Admin Stories_**](#admin-stories)
</details>

**<details><summary>UX</summary>**
* [**_Strategy Plane_**](#strategy-plane)
* [**_Scope Plane_**](#scope-plane)
* [**_Structure Plane_**](#structure-plane)
* [**_Skeleton Plane_**](#skeleton-plane)
* [**_Surface Plane_**](#surface-plane)
    * [_Color Scheme_](#color-scheme)
    * [_Typography_](#typography)
    * [_Media_](#Media)
    * [_Wireframes_](#wireframes)
</details>

**<details><summary>Features</summary>**
* [**_Existing Features_**](#existing-features)
* [**_Features Left to Implement_**](#features-left-to-implement)
</details>

**<details><summary>Technologies Used</summary>**
* [**_Libraries_**](#libraries)
* [**_Version Control_**](#version-control)
</details>

**<details><summary>Accessibility</summary>**
* [**_Semantics_**](#semantics)
</details>

**<details><summary>Testing</summary>**
* [**_Testing_**](#testing)
</details>

**<details><summary>Deployment</summary>**
* [**Deployment**](#deployment)
</details>

**<details><summary>Credits</summary>**
* [**_Content_**](#content)
* [**_Acknowledgements_**](#acknowledgements)
</details>

---

# Project Overview

BiaBook is a simple recipe website where users can share their recipes and view other's.
---

### User Stories

-  As a user, I would like to be able to search for recipes.
-  As a user, I would like to create a profile and upload a picture.  
-  As a user, I would like to view what recipes other users have created.
-  As a user, I would like to register in order to have my own account.
-  As a registered user, I would like to add, edit or delete my own recipes.


### Admin Stories

- As a site owner, I want to create a site that is mobile ready.
- As a site owner, I want to be able to add or remove categories.
- As a site owner, I want my users to be able to sign up to the website.
- As a site owner, I want my users to be able to connect with the owner/team via social media channels.
---

---

## UX Planes

### Strategy Plane

- Project Goals: The goal of this project was to create a simple website where users could share and view other recipes. They could create their very own account and learn new cuisines from other users.

- Content: The content is determined by the users and presented in a uniform and clear manner.

#### Personal Goals

- To learn and practice frontend and backend programming together for the first time. To combine the use of HTML, CSS, Materialize and JavaScript with Python, MongoDB, Flask and Jinja.

### Scope Plane

- A website where users can showcase their recipe with simplicity.
- A website with minimal but yet subtle interaction amongst the users.
- Future Technologies would be a fully interactive profile page for each user.


### Structure Plane
- Nav bar on each page with *Recipes*, *Login* and *Register* - *add recipe* is available once a member.
- Recipes: A showcase of user recipes with a search bar to aid users in finding a particular recipe.
- Login: Where the user can access their profile by supplying their username and password.
- Register: Where a user can sign up and begin sharing recipes.
- Footer: to the social media sites.

### Skeleton Plane
#### Wireframes

-  designed the site mock-ups using balsamiq wireframes. Each image/pdf shows a page and how the displays would change on different screen sizes such as mobile, tablet and desktop.

### Surface Plane

- limited fonts and colour scheme

#### Design

A standard layout is fully responsive on mobile devices and larger screens.

#### Color Scheme

Colors are kept to a minimum in order to keep focus on the imagery of the recipes, chosen colousr are various shades of grey. Color scheme can be found on my Coolors profile: [Coolors](https://coolors.co/u/sean_mcmahon)

![Color Palette](https://github.com/Sean-Mc-Mahon/McTasticRecipes/blob/master/wireframes/mctastic-colors.JPG)

#### Typography

 [Google Fonts](https://fonts.google.com/) were used across the site:

- [Vollkorn SC](https://fonts.google.com/specimen/Vollkorn+SC?selection.family=Reggae+One|Vollkorn+SC&sidebar.open=true&preview.text_type=custom) : Used throughout the entire site.

All images, and recipes are the authors own unless provided by other users. Logos are also produced by the author using Affinity Design.

- [Balsamiq Wireframe](https://github.com/Sean-Mc-Mahon/McTasticRecipes/blob/master/wireframes/mctastic-wire.pdf)

- [Affinity Designer Logo Process](https://github.com/Sean-Mc-Mahon/McTasticRecipes/blob/master/wireframes/logo-design.jpg)

##### back to [top](#table-of-contents)

---

# Features

## Existing Features

### Elements on every page
#### Navbar
- The navigation Bar.

- For visitors to the site who are not logged in, list items links are available for them to use.
    1. Recipes
    2. Register
    3. Login

- For users who are logged in, the list items are as follows: 
    1. Logout
    2. Add Recipes
    3. Profile
    4. Users

- Python determines if the user is logged in or not by checking `if 'user' in session` and passes this data to Jinja to display the correct navbar for the user.

- Using [Materializecss](https://materializecss.com/), on the smaller resolutions (tablet, mobile) the navbar collapses into a burger icon and opens from the side.

#### Footer

The Footer features:
- Contact section
- Copyright Information
- Links to social media platforms.

### Elements on Multiple Pages

#### Search Sort Filter 
(index, search, single_recipe)

- The index page has a search bar, filter and sort feature. The search feature searches for keywords in recipe titles and ingredients. If a user performs a search they will be able to sort the search results.
- The sort feature allows users to sort the results by A-Z, Z-A, latest created and oldest created.
- The filter allows users to display recipes under the categories of cooking, baking, snacks or all.

#### Recipe Cards 
(index, view_profile)

- Cards are displayed for each recipe. On small devices the cards may be expnded to reveal more information (one card per row on small devices, two cards per row on medium devices). <br>
- On large devices users can hover over cards to reveal more information (3 cards per row). <br>

#### Ingredient Cards 
(units, add_recipe)

- Cards are displayed for each ingredient. On small devices the cards may be expnded to reveal more information (one card per row on small devices, two cards per row on large devices). If logged in a user may add ingredients, if ingredient name does not already exist it will be entered. If a user created the ingredient they may edit or delete it. Admin user may see the creator of any ingredient and may delete any ingredient. 


### Individual Pages


### Recipes

- This page contains:
    - a view of recipes from all the users.
    - If signed in, you can edit or delete your recipe.
    - You can open each collapsible to view the recipe contents and it's image.

### Register

- This page contains a form where users may register and be redirected to their profile. Below the form is a link to login.

### Login

- This page contains a form where users may login and be redirected to their profile. Below the form is a link to register.

### Logout

- Clicking 'Logout' ends a user session and redirects them to the 'Login' page.



# Future Features to Implement

- **Image Hosting** 

    Each image added to the recipes comes from a http: link, in the future I would love to make it so the user would be able to upload an image to the database.

-   **Profile Page**

    - The Profile page currently allows users to upload an image but they are unable to save it. I would like to add this feature later.
    - Also, I would like to make a profile page similar to one you might find on [facebook](www.facebook.com) where user could design it to their tast and like and/ favourite other user's recipes.
    - I would like to add a video platform where users could vlog their recipes and have others follow their content.

    

##### back to [top](#table-of-contents)

# Technologies Used

- [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) - Used throughout the site.
- [CSS](https://www.w3.org/Style/CSS/Overview.en.html) - Used throughout the site.
- [JavaScript](https://www.javascript.com/) - Used to help features in [Materialize](https://materializecss.com/).
- [Materialize](https://materializecss.com/) - Used to aid responsive design and for componants such as modals.
- [Gitpod](https://code.visualstudio.com/) - Code Editor used to create the site.
- [GitHub](https://github.com/) - Used to host repos for the site.
- [Imgur](https://imgur.com/) - Used to host images for the site.

- [Chrome](https://developers.google.com/web/tools/chrome-devtools) - Used to test/ find a solution to a problem.
- [W3C Markup Validation Service](https://validator.w3.org/https://jigsaw.w3.org/) - Used to test code for errors.
- [Affinity Designer](https://affinity.serif.com/en-gb/) - Illustration software used to create logos and icons.

- [Balsamiq](https://balsamiq.com/?) - Used to create wireframes.
- [Tinypng](https://tinypng.com/) - Used to compress images.

- [Randomkeygen](https://randomkeygen.com/) - Used to generate random keys.
- [Kaffeine](https://kaffeine.herokuapp.com/) - Used to keep Heroku app from falling asleep.
- [Uptime Robot](https://uptimerobot.com/) - Used to keep Heroku app from falling.

### Libraries
ss.com/) - is a fr
- [Materialize](https://materializecamework for building responsive, mobile-first websites. 

- [JQuery](https://jquery.com/) - is a Javascirpt library. 

- [Flask](https://flask.palletsprojects.com/en/1.1.x/) - is a lightweight WSGI web application framework - used it to construct and render pages.

- [Jinja](https://flask.palletsprojects.com/en/1.1.x/) - is a templating language for Python - used to display data from the backend in HTML.

- [PyMongo](https://flask.palletsprojects.com/en/1.1.x/) - is the recommended way to work with MongoDB from Python - used to communicate between Python and MongoDB.

- [dnspython](https://pypi.org/project/dnspython/) - is a DNS toolkit for Python.

### Version Control

- [Git](https://git-scm.com/) - used for version control


---

# Accessibility

### Semantics

- HTML5 Semantics used throughout (header, nav, main etc...)
- Titles used throughout (McTastic Recipes, McTastic Profiles etc...)
- Language is set to english (`<html lang="en">`)

---

- Aria labels used throughout eg `<button id="submit" aria-label="submit" type="submit">`
- Alt Text: Alt text dynamically applied to images eg `alt="{{recipe.recipe_name}} image"`

# Testing
All testing and validation is contained within a separate .md file. <br> [View TESTING.md](TESTING.md)

# Deployment

1. This repository may be cloned directly into an editor by pasting the following command into the terminal:   
`git clone https://github.com/Sean-Mc-Mahon/McTasticRecipes`    
Alternatively, you can save a copy of this repository by clicking the green button "Clone or download" , then "Download Zip" button, and after extract the Zip file to your folder.
2. In the terminal window change directory (CD) to the correct file location (directory that you have just created).
3. Set up environment variables:
    - Create **.env** file in the root directory.
    - On the top of the file add `import os` to set the environment variables in the operating system.
    - Set the connection to your MongoDB database(MONGO_URI) and a SECRET_KEY with the following syntax:
    `os.environ["SECRET_KEY"] = "YourSecretKey"`   
    `os.environ["MONGO_URI"] = "YourMongoURI"`  
    .
4. Install all requirements from the **requirements.txt** file putting this command into your terminal:   
`pip3 install -r requirements.txt`  
*Note: GitPod does not require `sudo`, so if you use another IDE, you will need to include `sudo` in the beginning of the command: `sudo pip3 install -r requirements.txt`.*
5. Create a new Database called "recipe_manager" in [MongoDB Atlas](https://www.mongodb.com/).   
*You can sign up for free account, if you do not have one.*
6. In "recipe_manager" database create eight following collections:
###### categories
```
_id: <ObjectId>
category_name: <String>
```

###### Recipes
```
_id: <ObjectId>
category_name: <String>
recipe_name: <String>
recipe_ingredients: <String>
recipe_method: <String>
recipe_image: <String>
created_by: <String>

```

###### users
```
_id: <ObjectId>
username: <String>
password: <String>
```
7. You will now be able to run the application using the following command `python3 app.py`. 

### Heroku Deployment
To deploy the project to [Heroku](https://heroku.com/) the following steps need to be completed:
1. Create a **requirement.txt** file, which contains a list of the dependencies, using the following command in the terminal:  
`pip3 freeze > requirements.txt`
2. Create a **Procfile**, in order to tell Heroku how to run the project, using the following command in the terminal:   
`echo web: python run.py > Procfile`
3. `git add`, `git commit` and `git push` these files to GitHub repository
4. Create a **new app** in Heroku, assigning a name (must be unique) and set a region (for my project I set Europe)
5. From the Heroku dashboard link the new Heroku app to your GitHub repository:    
    - "Deploy" -> "Deployment method" -> "GitHub"
    - then "Enable automatic deployment"
6. To start the web process, put the following command into the terminal: `heroku ps:scale web=1` to scale dynos
7. In the **Settings** tab of the new Heroku app, click on "Reveal Config Vars" and set the following config vars:
    - **IP** : 0.0.0.0
    - **PORT** : 5000
    - **MONGO_URI** : `<link to your MongoDB database>`
    - **SECRET_KEY** : `<your secret key>`
    - **DEBUG**: **FALSE**  
*Note: your MONGO_URI and SECRET_KEY must match the ones you entered in 'env.py' file*

8. The app will be deployed and ready to run. Click "Open App" to view the app.   

**Note**: if you have not linked GitHub and Heroku following step **5**, alternatively as the last step of deployment, you can put the following command into your terminal:   
 `heroku login`, after a successful log in `git push heroku master` - to push the app to Heroku, and finally click "Open App" in Heroku dashboard to view the app.

---

# Credits

### Content

1.  Google Fonts for font styles; https://fonts.google.com/

2.  Youtube; Various resources for Materialize taken from [The Net Ninja](https://www.youtube.com/playlist?list=PL4cUxeGkcC9gGrbtvASEZSlFEYBnPkmff)

3.  Youtube; Code for temperature conversion modified from [Whatsdev](https://youtu.be/EHclqGV_KME)

4.  Youtube; Code for temperature conversion modified from [Whatsdev](https://youtu.be/EHclqGV_KME)

5.  Github; Code for pagination modified from [irinatu17](https://github.com/irinatu17/MyCookBook)

6.  Github; Code for url validation and placehoder image modified from [Paulloy](https://github.com/paulloy/whiskey_herald_msp3/blob/master/app.py)

7.  Github; Format of README modified from [Mr-Smyth](https://github.com/Mr-Smyth/circles/blob/master/README.md) and [irinatu17](https://github.com/irinatu17/MyCookBook/blob/master/README.md)

7.  Icons sourced from [Iconmonstr](https://iconmonstr.com/)

8.  Button icons sourced from [Fontawesome](https://fontawesome.com/)

 

### Acknowledgements

1.  My mentor Adegbenga Adeye for his support and input.

2.  My peers on slack for their generosity in sharing their knowledge and experience.

---

This project is for educational use only

##### back to [top](#table-of-contents)