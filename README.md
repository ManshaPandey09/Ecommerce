#  Mini Market Ecommerce Project

A full-stack mini e-commerce web app where users can browse products, manage their cart, sign in, post products, and update profiles. The frontend is built with HTML, CSS, and JavaScript, while the backend uses Java Servlets and MySQL. Product data is dynamically loaded via Google Sheets using SheetDB, and Firebase handles user authentication.

---

##  Features

###  Frontend
-  Dynamic Product Listing (via Google Sheets + SheetDB)
-  Add to Cart with live cart count
-  Coupon code support
-  Fully responsive UI using HTML/CSS/JavaScript

###  Backend (Java)
-  Firebase Authentication Integration
-  User profile creation & update via Servlets
-  Product posting system (via form & Java Servlet)
-  MySQL database for storing posted products
-  Fetch user’s own posted products on profile page

---

##  Folder Structure (Simplified)

minimarket/
├── css/
├── js/
├── img/
├── src/
│ ├── model/ # Java model classes
│ ├── dao/ # DAO classes for MySQL operations
│ ├── servlet/ # Java Servlets (AddProductServlet, etc.)
│ ├── util/ # DB connection utils
├── WEB-INF/
│ ├── web.xml # Servlet config
│ ├── lib/ # MySQL connector .jar
│ ├── classes/ # Compiled Java .class files
├── index.html
├── cart.html
├── login.html
├── signup.html
├── profile.html
├── sproduct.html
├── README.md


---

##  Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Java (Servlets)
- **Database**: MySQL
- **Authentication**: Firebase Auth
- **External API**: SheetDB (to pull products from Google Sheets)
- **Server**: Apache Tomcat

---

##  How to Run the Project

###  Frontend Only:
1. Open `index.html` in a browser
2. Internet is required for Firebase & SheetDB to work

###  Full Stack (Java Backend + MySQL):

1. Import the project into Eclipse or VS Code with Java support
2. Make sure MySQL is installed and running
3. Create a database:
    ```sql
    CREATE DATABASE minimarket;
    ```
4. Update DB credentials in `DBUtil.java`
5. Place MySQL connector `.jar` in `WEB-INF/lib/`
6. Compile using:
    ```bash
    javac -cp "WEB-INF/lib/*" -d WEB-INF/classes src/**/*.java
    ```
7. Deploy the project to Apache Tomcat


---


## GitHub Repository

[https://github.com/ManshaPandey09/Ecommerce](https://github.com/ManshaPandey09/Ecommerce)

---

## Contributors

- Mansha Pandey – Full Stack Developer

