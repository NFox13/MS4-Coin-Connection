# Coin Connection

[![Coin Connection Logo](media/logo.jpg)]( https://ms4-coin-connection.herokuapp.com/)

Coin Connection is an e-commerce website for people to buy bullion or antique coins. The site is not directed entirely to numismatists but to people who may want to buy coins as an investment also.

- [UX](#ux)
  - [Project Goal](#project-goal)
  - [User Stories](#user-stories)
    - [User Stories for Customers](#user-stories-for-customers)
    - [User Stories for Administrators](#user-stories-for-admin)
  - [Wireframes](#wireframes)
  - [Data Structure](#data-structure)
  - [Design](#design)
    - [Typography](#typography)
    - [Colours](#colours)
- [Features](#features)
  - [Existing Features](#existing-features)
    - [Home Page](#home-page)
    - [Product Page](#product-page)
    - [Product View](#product-view)
    - [User's Profile Page](#profile-page)
    - [User Login and Sign-Up](#user-account)
    - [Shopping Bag](#shopping-bag)
    - [Secure Checkout](#secure-checkout)
    - [Administrator features](#admin-features)
  - [Possible Future Features](#possible-future-features)
- [Testing](#testing)
- [Deployment](#deployment)
  - [Local Deployment](#local-deployment)
  - [Deployment to Heroku](#deployment-to-heroku)
- [Technologies](#technologies)
- [Tools Used](#tools)
  - [Design Library](#design-library)
- [Known Bugs](#known-bugs)
- [Version Control](#version-control)
- [Credits](#credits)
  - [Media](#media)
  - [Acknowledgements](#acknowledgements)

---

Welcome to Coin Connection - the e-commerce website for Numismatists and investors to purchase antique and bullion coins. Users will be able to register/login, create a profile and purchase coins.

Access the site: <https://ms4-coin-connection.herokuapp.com/>

[![Am-I-Responsive](media/responsive.jpg)](https://ms4-coin-connection.herokuapp.com/)


### Project Goal

This is my fourth and final Milestone Project in Code Institute's Fullstack Development program. The purpose of this project was to create an e-commerce site using the Django framework, static file hosting with AWS, and a functional payment system with Stripe. The e-commerce section of the site is fully functional, Stripe payments and webhooks are operational and all static files, including media (images) are located at Amazon Web Services (AWS). I think the site has great potential to grow with additional features to be added in the future.

My site was inspired by Code Institute's tutorials for the Boutique Ado project: [Boutique Ado Code](https://github.com/Code-Institute-Solutions/boutique_ado_v1/)

## UX

### User Stories

#### User Stories for Customers

User Stories for Customers at [Coin Connection](<(https://ms4-coin-connection.herokuapp.com/)>)
A customer would like to: | Page(s) associated:
--- | --- 
Browse for coins | <https://ms4-coin-connection.herokuapp.com/products/>
Register using email | <https://ms4-coin-connection.herokuapp.com/accounts/signup/>
Login to an account using email | <https://ms4-coin-connection.herokuapp.com/accounts/login/>
Search coins | <https://ms4-coin-connection.herokuapp.com/products/?q=gold>
Sort coins based on categories | <https://ms4-coin-connection.herokuapp.com/products/?sort=category&direction=asc>
Sort coins by region | <https://ms4-coin-connection.herokuapp.com/products/?sort=region&direction=asc>
Sort coins by material | <https://ms4-coin-connection.herokuapp.com/products/?sort=material&direction=asc>
Sort coins by price | <https://ms4-coin-connection.herokuapp.com/products/?sort=price&direction=asc>
Read coin descriptions | <https://ms4-coin-connection.herokuapp.com/products/2/>
Buy a coin/coins and view in a shopping cart before purchase | <https://ms4-coin-connection.herokuapp.com/bag/>
Update the number of items in the shopping cart before purchase | <https://ms4-coin-connection.herokuapp.com/bag/>
Know how much delivery will cost and when the free delivery threshold activates | <https://ms4-coin-connection.herokuapp.com/bag/>
Pay by using a credit card in from a safe and reputable source | <https://ms4-coin-connection.herokuapp.com/checkout/>
Buy a coin and have the item delivered to a confirmed address | <https://ms4-coin-connection.herokuapp.com/checkout/>
Create a profile | <https://ms4-coin-connection.herokuapp.com/profile/>
Review order history | <https://ms4-coin-connection.herokuapp.com/profile/>
Update profile information | <https://ms4-coin-connection.herokuapp.com/profile/>

#### User Stories for Coin Connection Administrators/Superuser

Admin Stories for site administrators at [Coin Connection](<(https://ms4-coin-connection.herokuapp.com/)>)
-- _note: some pages may not be accessible without being an administrator or superuser. Request access via email_
An admin would like to: | Page(s) associated:
--- | ---
Add a product | <https://ms4-coin-connection.herokuapp.com/products/add/> -- (only viewable when logged in as an administrator/Superuser)
Update a product | <https://ms4-coin-connection.herokuapp.com/products/3/> -- (only viewable when logged in as an administrator/Superuser)
Delete a product | <https://ms4-coin-connection.herokuapp.com/products/3/> -- (only viewable when logged in as an administrator/Superuser)

- _The above details the types of actions an administrator/Superuser can do from the website, however, all administrators/Superuser will also have access to the database through Django's admin panel._


### Wireframes

Following the user stories, wireframes were drawn to provide a starting point and guidance throughout the development process. Some minor changes occurred during production but I kept the design to the Boutique Ado design as it works well.

#### Desktop Wireframes

The home page on desktop
![Coin Connection Desktop Wireframe](media/home-desktop.jpg)

The products page on desktop
![Coin Connection Desktop Wireframe](media/products-desktop.jpg)

#### Mobile Wireframes

The home page on mobile
![Coin Connection Mobile Wireframe](media/home-mobile.jpg)

The products page on mobile
![Coin Connection Mobile Wireframe](media/products-mobile.jpg)

To aid the user experience, the pages follow the same design. Navigation, menu options etc are carried through in each page.


### DESIGN

The application was built using Bootstrap. The font, colours and design were all chosen to give a sleek, clean and clear look to the site.
The responsiveness was developed so users can have a pleasant experience on desktop, laptop, tablet or mobile.

#### Typography

The google font "Poppins" regular 400 was used throughout the site, again to give a sleak look and it is easy to read: <https://fonts.google.com/specimen/Poppins>
The site also uses [Fontawesome](https://fontawesome.com/) icons throughout.

#### Colours

Colours were chosen to best reflect to clean look of black and white along with the silver and gold of bullion.
The colour scheme was generated using [Coolors](https://coolors.co/)
![Colour scheme](media/colour-scheme.jpg)



