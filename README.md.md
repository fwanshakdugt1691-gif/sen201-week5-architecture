\# SEN201 - Week 5 Lab: Software Architecture \& Design Pattern Exploration



\## Online Course Management System Architecture



\### Chosen Architectural Style

\*\*Layered Architecture (N-Tier Architecture)\*\* combined with \*\*MVC (Model-View-Controller)\*\* pattern at the presentation and application layers.



\### Justification



The Layered Architecture is the most suitable choice for the initial design of the Online Course Management System. This style organizes the system into distinct horizontal layers (Presentation, Application/Business Logic, Domain, and Data Persistence), each with clear responsibilities and dependencies flowing in one direction (typically downward). This separation aligns perfectly with the key requirements of \*\*maintainability\*\* and \*\*scalability\*\*.



For maintainability, changes in one layer (e.g., updating the user interface or switching the database) have minimal impact on other layers, making it easier to update and extend features without breaking existing functionality. This is especially important for an educational system that will likely evolve over time with new features like discussion forums, live classes, or analytics dashboards.



Regarding scalability, the layered approach allows horizontal scaling of specific layers independently. For example, the web/presentation layer can be scaled to handle increasing numbers of concurrent students during peak registration periods, while the data layer can be optimized separately. Security is also enhanced because sensitive operations (authentication, authorization, and data access) can be strictly controlled in the Application and Domain layers.



Additionally, incorporating the \*\*MVC pattern\*\* within the Presentation and Application layers provides a clean separation between the user interface, business logic, and data representation. This improves usability by allowing frontend developers to work on responsive, intuitive interfaces independently from backend logic, while ensuring a consistent user experience for students, instructors, and admins.



Overall, Layered + MVC offers a balanced, robust foundation that supports the system's security needs, data persistence requirements, and future growth without introducing unnecessary complexity for the initial implementation.





