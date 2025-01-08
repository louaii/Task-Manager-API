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



