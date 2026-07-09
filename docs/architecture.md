# Software Architecture

## Overview

For this project, we chose the **Layered Architecture** because it provides a good balance between simplicity and maintainability. It is well suited for a medium-sized application like this password manager, offering clear separation of responsibilities, good testability, and flexibility for future growth. Compared to more complex architectures such as Clean Architecture, it introduces less unnecessary complexity while still following professional software engineering practices.

## Dependency Rules

To improve maintainability, reduce coupling, and minimize the impact of future changes, communication between layers is restricted.

The UI layer communicates only with the Application layer.

The Application layer coordinates the system and is allowed to interact with both the Domain and Infrastructure layers.

The Domain layer contains the core business logic and must remain independent of the UI and Infrastructure.

The Infrastructure layer is responsible for external resources such as the database, file system, encryption, and clipboard, and should not depend on the UI.

## Technology Stack

Language                Python 3.14         زبان اصلی پروژ
GUI                     Pyside6             رسمی، قدرتمند، رایگان (LGPL)، مناسب پروژه‌های حرفه‌ای
Database                SQLite              سبک، آفلاین و بدون نیاز به سرور
Encryptin               Creyptography       استاندارد و امن، از ساخت رمزنگاری اختصاصی جلوگیری می‌کند
Testing                 pytest              استاندارد اکوسیستم پایتون
Dependency Mnagement    uv                  سریع، مدرن و جایگزین مناسب pip
Code Formatting         Ruff                فرمت‌کننده و Linter بسیار سریع
Version Control         Git + GitHub        مدیریت نسخه و انتشار پروژه