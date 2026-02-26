🎮 Game Rental Database Model
📌 Project Overview

This project presents the logical data modeling (ERD) of a digital game rental system.

The objective was to design a relational database structure capable of handling:

Customer registration

Game catalog management

Rental transactions

Many-to-many relationships between rentals and games

The model was developed using DBML (Database Markup Language) and designed following relational database best practices.

🏗 Database Structure
Entities

clientes – Stores customer data

jogos – Stores game catalog information

locacoes – Stores rental transactions

itens_locacao – Associative table resolving the N:N relationship

🔗 Relationships

1:N → One customer can have multiple rentals

1:N → One rental can contain multiple games

1:N → One game can appear in multiple rentals

N:N → Rental ↔ Game (resolved through itens_locacao)

🧠 Design Decisions

Use of a composite primary key in the associative table

Separation of business entities to maintain normalization

Referential integrity through foreign keys

Avoidance of redundancy via many-to-many resolution

This model follows 3NF principles.

🛠 Technologies Used

DBML

dbdiagram.io

Relational Database Modeling Concepts

📎 DBML Code

(cole o código aqui)

📈 Possible Improvements

Add rental status control

Implement pricing structure

Introduce payment tracking

Add constraints for business rules enforcement
