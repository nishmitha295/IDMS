# IDMS - Internal Data Management System

A centralized data management platform for internal departments such as HR, Store, Attendance, Memo, Finance, and Reports. Built with a modern tech stack (Next.js + Spring Boot), IDMS enables role-based access, secure data workflows, and smooth collaboration across teams.

---

## 🚀 Features

* **User Authentication**: JWT-based login and secure session handling
* **Role-based Access**: Admin, Employee, HR, Store Manager, Finance roles
* **Department Dashboards**: Custom views for HR, Finance, Store, and Admin
* **Attendance Tracking**: Daily in/out status and leave management
* **Asset Management**: Manage office assets (printers, furniture, etc.)
* **Finance Manager**: Track fixed and variable expenses
* **Memo & Notices**: Create and distribute internal memos
* **Performance Tracker**: Track employee KPIs and appraisal data
* **Reports Generation**: Department-wise internal reports
* **Responsive UI**: Clean and intuitive design for desktop and mobile

---

## 🛠 Tech Stack

### Frontend (NewIDMS-project)

* **Next.js** – Server-side rendering React framework
* **TypeScript** – Static typing
* **Tailwind CSS** – Modern UI styling
* **Axios** – API communication
* **Lucide Icons** – Icon pack
* **React Hot Toast** – Toast notifications

### Backend (BackendNewWorkManagement)

* **Spring Boot** – Java-based backend framework
* **MySQL** – Relational database
* **JWT** – Authentication
* **REST API** – Secure endpoints for each module
* **Spring Security** – Role and session management

---

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/nishmitha295/IDMS.git
cd IDMS
```

---

### 2. Backend Setup

```bash
cd BackendNewWorkManagement
```

* Configure `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/idms
spring.datasource.username=root
spring.datasource.password=your_password
```

* Run the Spring Boot App:

```bash
mvn spring-boot:run
```

---

### 3. Frontend Setup

```bash
cd ../NewIDMS-project
npm install
```

* Configure `.env.local`:

```env
NEXT_PUBLIC_API_BASE_URL=http://localhost:8080/api
```

* Start the Dev Server:

```bash
npm run dev
```

---

## 🌐 API Endpoints

### Authentication

* `POST /api/auth/login` – User login
* `POST /api/auth/register` – Register new users
* `GET /api/auth/me` – Get profile details

### HR

* `GET /api/hr/employees` – List employees
* `POST /api/hr/documents` – Upload or view HR docs
* `PUT /api/hr/leave` – Apply or approve leaves

### Store

* `GET /api/store/assets` – View/store assets
* `POST /api/store/transfer` – Manage transfers

### Finance

* `GET /api/finance/expenses/fixed`
* `GET /api/finance/expenses/variable`

### Memo

* `POST /api/memo/send` – Send memo
* `GET /api/memo/list` – View all memos

---

## 🧩 Project Structure

```
IDMS/
├── BackendNewWorkManagement/   # Java Spring Boot Backend
└── NewIDMS-project/            # Next.js React Frontend
```

---

## 🔒 Security Features

* JWT Authentication with refresh tokens
* Role-based access for each department
* Protected frontend routes with role guards
* Input validation and exception handling

---

## 📸 Screenshots

> *You can add UI screenshots here to show login page, dashboards, etc.*

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👩‍💻 Author

* **Nishmitha M V** – Full Stack Developer
