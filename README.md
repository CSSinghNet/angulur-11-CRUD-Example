# angular-11-crud-example

Angular 11 - CRUD Example with Reactive Forms

# Introduction

Angular 11 CRUD application with Reactive Forms that includes pages for listing, adding, editing and deleting records from a JSON API. The records in the example app are user records, but the same CRUD pattern and code structure could be used to manage any type of data e.g. products, services, articles etc.

# Fake backend API with CRUD routes

The example app runs with a fake backend api by default to enable it to run completely in the browser without a real api (backend-less), the fake api contains routes for user CRUD operations (Create, Read, Update, Delete) and it uses browser local storage to save data. To disable the fake backend you just have to remove a couple of lines of code from the app.module.ts file, you can refer to the fake backend to see what's required to build a real api for the example.

# Example CRUD App Overview

The example app includes a basic home page and users section with CRUD functionality, the default page in the users section displays a list of all users and includes buttons to add, edit and delete users. The add and edit buttons navigate to a page containing an Angular Reactive Form for creating or updating a user record, and the delete button executes a function within the user list component to delete a user record. The add and edit forms are both implemented with the same add/edit component which behaves differently depending on which mode it is in ("add mode" vs "edit mode").