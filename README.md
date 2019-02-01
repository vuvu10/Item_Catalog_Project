# Item_Catalog_Project

> Vuvu Siona

## About

This is the project for the Udacity Full Stack Nanodegree. The Item Catalog project consists of developing an application that provides a list of items within a variety of categories, as well as provide a user registration and authentication system. This project uses persistent data storage to create a RESTful web application that allows users to perform Create, Read, Update, and Delete operations.

A user does not need to be logged in in order to read the categories or items uploaded. However, users who created an item are the only users allowed to update or delete the item that they created.

This program uses third-party auth with Google or Facebook. Some of the technologies used to build this application include Flask, Bootsrap, Jinja2, and SQLite.


## Skills used for this project
- Python
- HTML
- CSS
- Bootstrap
- Flask
- Jinja2
- SQLAchemy
- OAuth
- Facebook / Google Login

## Some things you might need
- [Vagrant](https://www.vagrantup.com/)
- [Udacity Vagrantfile](https://github.com/udacity/fullstack-nanodegree-vm)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## Getting Started

- Install Vagrant and VirtualBox
- Clone the Vagrantfile from the Udacity Repo
- Clone this repo into the `catlog/` directory found in the Vagrant directory
- Run `vagrant up` to run the virtual machine, 
- Run `vagrant ssh` to login to the VM
- Rum `cd /vagrant` to get into the vagrant directory and the go to the catalog directory
- From the main directory run `sudo pip install -r requirements.txt`, this will install all the dependencies of the project
- Run application with `python application.py` from within its directory
- Now you can access the application on `http://localhost:5000/`
- *if first time running, you must add a category before adding an item

## Using Google Login
To get the Google login working there are a few additional steps:

1. Go to [Google Dev Console](https://console.developers.google.com)
2. Sign up or Login if prompted
3. Go to Credentials
4. Select Create Crendentials > OAuth Client ID
5. Select Web application
6. Enter name 'Item-Catalog'
7. Authorized JavaScript origins = 'http://localhost:5000'
8. Authorized redirect URIs = 'http://localhost:5000/login' && 'http://localhost:5000/gconnect'
9. Select Create
10. Copy the Client ID and paste it into the `data-clientid` in login.html
11. On the Dev Console Select Download JSON
12. Rename JSON file to client_secrets.json
13. Place JSON file in item-catalog directory that you cloned from here
14. Run application using `python /item-catalog/app.py`

## Know issues

- No validation on forms

## Possible improvements

- Add an additional data model so that users can add Stores
- Image Upload, possible future addition with file upload
- Styling and layout could improve
- Implement CSRF protection on CRUD operations.
