Clean Architecture .NET Backend Boilerplate

Ett återanvändbart backend-startprojekt byggt med Clean Architecture i .NET.
Projektet innehåller JWT-autentisering, EF Core + SQL och ett tydligt lagerupplägg för skalbara applikationer.

Projektstruktur
├── API/               → Controllers, Requests, Responses, DI
├── Application/       → Use Cases, DTOs, Services, Interfaces
├── Domain/            → Entities, Value Objects, Domain Rules
├── Infrastructure/    → EF Core, SQL, Repository Implementations
├── Test/              → Unittester (om tillagt)
└── Clean-API.sln

Arkitektur
Lager	Ansvar
Domain	Entiteter, logik, regler
Application	Use cases, DTOs, services
Infrastructure	Databas, EF Core, Repositories
API	Controllers, routing, authentication

✔ API kommunicerar aldrig direkt med databasen
✔ All logik passerar via Application-lagret
