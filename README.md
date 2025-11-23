### Event Management System

A web-based Event Management System built with Java Servlets/JSP, HTML, CSS, JavaScript, and MySQL. It enables admins/managers to manage events and users to browse, book, and pay for events.

### Features
- **User accounts**: Registration, login, logout, profile management
- **Role-based dashboards**: Admin/Manager views
- **Event management**: Create, update, delete, and list events
- **Bookings**: Reserve/book events, view bookings
- **Payments**: Add/update/delete payments, view payment history
- **Feedback**: Submit, list, update, and delete feedback
- **Search & filters**: Find events by category/date
- **JSP views**: Pages for login, register, events, admin, and more

### Tech Stack
- **Backend**: Java (Servlets/JSP), JDBC, JSTL
- **Frontend**: HTML, CSS, JavaScript
- **Database**: MySQL
- **App Server**: Apache Tomcat (or any Servlet 3.x compatible)

### Getting Started
1. Clone the repository
2. Set up a local server (Tomcat via Eclipse/IntelliJ or standalone Tomcat)
3. Create a MySQL database and import SQL:
   - SQL file: `src/main/webapp/Database/mycrud.sql`
4. Update DB credentials:
   - `src/main/java/utility/DBUtil.java`
   - `src/main/java/EventBookingPackage/DBConnection.java`
   - `src/main/java/FeedbackPackage/DBConnection.java`
5. Ensure required JARs exist in `src/main/webapp/WEB-INF/lib`:
   - `mysql-connector-java`, `servlet-api`, `jstl`
6. Deploy and run on Tomcat:
   - Eclipse: Import as a Dynamic Web Project → Run on Server
   - Standalone Tomcat: Build an exploded WAR and deploy to `webapps/`
7. Access the app:
   - `http://localhost:8080/<your-app-context>/` (e.g., `index.jsp`, `login.jsp`, `events.jsp`)

### Folder Structure
- `src/main/java/controller` – Event controllers/servlets
- `src/main/java/com/user` – Auth and payment servlets
- `src/main/java/dao` – Data access layer (JDBC queries)
- `src/main/java/model` – POJOs (`Event`, `User`, `Payment`, etc.)
- `src/main/java/utility` – DB utilities (`DBUtil`, `UserDBUtil`, `PaymentDBUtil`)
- `src/main/java/EventBookingPackage` – Booking controllers/servlets
- `src/main/java/FeedbackPackage` – Feedback controllers/servlets
- `src/main/webapp` – JSP pages and static assets
  - `Css/` – Stylesheets
  - `Javascript/` – Frontend scripts
  - `Images/` – Image assets
  - `WEB-INF/lib/` – App dependencies (JARs)

### License
This project is for educational purposes.
