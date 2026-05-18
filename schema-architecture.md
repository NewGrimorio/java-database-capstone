Questa applicazione Spring Boot utilizza sia controller MVC che REST. 
I template Thymeleaf sono utilizzati per i dashboard di Amministratore e Medico, mentre le API REST servono tutti gli altri moduli.
L’applicazione interagisce con due database: MySQL (per i dati di pazienti, medici, appuntamenti e amministratori) e MongoDB (per le prescrizioni). 
Tutti i controller instradano le richieste attraverso un layer di servizio comune, che a sua volta delega ai repository appropriati.
MySQL utilizza entità JPA mentre MongoDB utilizza modelli di documento.

Spero di fare un buon lavoro mentre lavoro a questo progetto.

1. Gli utenti accedono alla AdminDashboard e i medici accedono alla DoctorDashboard
2. Questa azione si effettua usando i Thymeleaf Controllers
3. Il controller Thymeleaf utilizza il ServiceLayer per instradare le richieste
4. Il service Layer utilizza le repository MySQL
5. Con le repository MySQL si accede al database MySQL
6. Il database MySQL accede ai modelli MySQL
7. Usiamo JPA Entity per MySQL (Patient,Doctor,Appointment,Admin)


English Version

Here is the translation:

---

This Spring Boot application uses both MVC and REST controllers.
Thymeleaf templates are used for the Administrator and Doctor dashboards, while REST APIs serve all other modules.
The application interacts with two databases: MySQL (for patient, doctor, appointment, and administrator data) and MongoDB (for prescriptions).
All controllers route requests through a common service layer, which in turn delegates to the appropriate repositories.
MySQL uses JPA entities while MongoDB uses document models.
I hope to do a good job while working on this project.

1. Users access the AdminDashboard and doctors access the DoctorDashboard
2. This action is performed using the Thymeleaf Controllers
3. The Thymeleaf controller uses the ServiceLayer to route requests
4. The Service Layer uses the MySQL repositories
5. The MySQL repositories are used to access the MySQL database
6. The MySQL database accesses the MySQL models
7. We use JPA Entity for MySQL (Patient, Doctor, Appointment, Admin)
