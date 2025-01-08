# Task-Manager-API
<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>


## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Introduction
The Task Manager API is a backend application developed with the Laravel framework, focusing on efficient task management through well-defined API endpoints. This project supports user registration, profile management, task creation, and categorization, all built on robust database relationships.

## Key Features:
User Registration and Authentication:

Secure mechanisms for user registration and login, ensuring data privacy and individualized task management.
Task Management:

CRUD operations on tasks, with each task containing attributes like title, description, and priority (High, Medium, Low).
Profile Management:

Each user can have one profile containing additional personal information such as address, date of birth, and bio.
Category Management:

Tasks can be categorized under multiple categories, allowing for flexible organization and retrieval.

## Database Relations:
### One-to-One Relationship:
User ↔ Profile:

A user can have exactly one profile.
The Profile model contains personal details and is linked to the User model through the user_id foreign key.

![Diagram_Task_Manager_1](https://github.com/user-attachments/assets/4281a031-b2a3-4458-902a-ddb7f9bc36c1)


### One-to-Many Relationship:
User ↔ Tasks:

A user can have one or many tasks.
The Task model includes task-specific details and links back to the User model via the user_id foreign key.

![Diagram_Task_Manager_2](https://github.com/user-attachments/assets/8013e191-d85f-41a1-9dc4-d6ec15ec066a)

### Many-to-Many Relationship:
Task ↔ Categories:

A task can belong to multiple categories, and a category can include multiple tasks.
This relationship is facilitated by a pivot table category_task with foreign keys linking tasks and categories.

![Diagram_Task_Manager_3](https://github.com/user-attachments/assets/ca15e8cd-21a2-40f7-bbd1-104a38d85dcb)

### Diagram:

![Full_Diagram](https://github.com/user-attachments/assets/a109f98e-ffcc-4bb2-86ac-cd47fa730149)


### Benefits:
Comprehensive User Management:

Profiles enrich the user experience by storing additional personal information.
Efficient Task Organization:

Tasks are not only managed by individual users but also categorized for easier retrieval and organization.
Scalable and Modular Design:

Built with Laravel’s modular structure, the API is scalable and maintainable, supporting future feature expansions and increasing user base.

### Conclusion:
The Task Manager API provides a powerful backend solution for task management applications, featuring secure user and profile management, prioritized task handling, and flexible categorization. Leveraging Laravel’s robust framework, it ensures high scalability, maintainability, and seamless integration with front-end systems.
