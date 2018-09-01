# notification-test
# Notification Developer Test (Symfony2/Backbone)

This project tests a developer's ability to read and write clean and maintainable code using relevant technologies. The project uses the following technologies:
* Symfony 2.8
* Backbone.js
* RequireJS
* SCSS
* Grunt

The goal of this project is to display new notifications to users on the base route of the project. The data structures and methods for adding/editing notifications have already been implemented on the **/list** route.

### Task

The task is to implement the following functionality on the default route of the web application. The front-end Backbone view should poll the server every minute and render any new valid (server time within the valid date range), active notifications to the user. Notifications should display the title and message, with new messages appearing above older ones. The server should track which notifications have been shown to the user through the user session, not displaying any duplicate notifications on page reload. Rendered notifications should be dismissable and fade away on-click. The page styling should be mobile responsive and implemented through SCSS.

## Getting Started

### Prerequisites

* php with the php-sqlite3 module
* composer
* npm

### Installing


Install all relevant PHP libraries with composer

```
composer install
```

Install all Grunt build tools with npm

```
npm install
```

Ensure grunt is running when making modifications in the project /assets directory.

```
grunt watch
```

Confirm the **app/data** directory has write permissions and your Symony2 instance has permissions to write to **app/cache** and **app/logs**.
