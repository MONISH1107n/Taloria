# TALORIA — Where Talent Finds Its Stage

## 📌 Project Overview

**TALORIA** is a sports talent discovery and opportunity platform designed to address the lack of visibility and opportunities faced by talented athletes.

Many athletes possess the skills and potential to succeed but struggle to reach scouts, coaches, tournament organizers, and suitable opportunities. TALORIA provides a centralized platform where athletes can showcase their abilities, participate in tournaments, and gain recognition through their performance.

The platform connects athletes, scouts, tournament organizers, and sponsors in one system. Sponsors support tournaments rather than individual athletes, creating more opportunities for players to participate and demonstrate their talent.

**Tagline:** *Where Talent Finds Its Stage.*

## 🎯 Objectives

- Provide athletes with a platform to showcase their skills and achievements.
- Improve athlete visibility among scouts and coaches.
- Enable athletes to discover and participate in tournaments.
- Help tournament organizers manage events and applications.
- Enable sponsors to support tournaments through sponsorship packages.
- Provide profile verification and transparent application tracking.
- Make sports talent discovery more accessible, structured, and transparent.

## ✨ Key Features

### 1. Athlete Module

- Register and manage athlete profiles.
- Add sports, skills, achievements, and performance statistics.
- Upload profile pictures and performance videos.
- Browse tournaments and apply for participation.
- Track application status and tournament history.
- Receive notifications about important activities.

### 2. Scout Module

- Search and filter athletes by sport, position, location, and performance.
- View athlete profiles, statistics, and achievements.
- Compare measurable performance statistics.
- Shortlist promising athletes.
- Maintain scouting notes and manage discoveries.
- Contact athletes through the platform, where implemented.

### 3. Tournament Management

- Create and publish tournaments.
- Define eligibility criteria, location, dates, and registration deadlines.
- Manage applications and participants.
- Approve or reject applications.
- Record tournament results and athlete performances.
- Track tournament status from publication to completion.

### 4. Sponsor Module

- Create and manage sponsor profiles.
- Browse available tournaments.
- Select sponsorship packages.
- Submit and track sponsorship requests.
- View sponsored tournament details.
- Track sponsorship status and history.

### 5. Administrator Module

- Manage users and platform activities.
- Review athlete verification requests.
- Manage tournaments and sports categories.
- Monitor applications and sponsorship requests.
- Review reports and uploaded content.
- Suspend users when necessary.

### 6. Search and Notifications

- Search and filter athletes and tournaments.
- Sort and paginate search results.
- Track application and sponsorship updates.
- Receive notifications about important activities.
- Manage saved tournaments and shortlisted athletes.

## 🔄 Core Workflow

**Discover → Participate → Perform → Get Discovered**

1. Athletes create profiles and showcase their abilities.
2. Tournament organizers publish tournaments.
3. Athletes discover tournaments and submit applications.
4. Organizers review applications and select participants.
5. Athletes participate and demonstrate their performance.
6. Scouts discover and shortlist athletes based on profiles and measurable statistics.
7. Sponsors support tournaments to create more opportunities for participation.

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | Python |
| Database | PostgreSQL |
| Database Queries | SQL |
| Architecture | Three-tier architecture |
| API Design | REST API |
| Development Methodology | Agile Scrum |

## 🏗️ System Architecture

TALORIA follows a three-tier architecture.

### 1. Presentation Layer

Provides the user interface, forms, dashboards, search pages, and tournament listings using HTML, CSS, and JavaScript.

### 2. Application Layer

The Python backend handles authentication, authorization, profile management, tournament workflows, applications, search and filtering, sponsorships, and notifications.

### 3. Database Layer

PostgreSQL stores and manages user accounts, athlete profiles, tournaments, applications, results, sponsorships, verification requests, and notifications.

**Architecture Flow:**

`User Interface → Python Backend/API → PostgreSQL Database`

## 🗄️ Database Design

TALORIA uses PostgreSQL, a relational database management system, to store and manage application data.

The planned database entities include:

- Users and Roles
- Athlete Profiles
- Scout Profiles
- Organizer Profiles
- Sponsor Profiles
- Sports and Athlete Skills
- Athlete Statistics
- Achievements and Performance Videos
- Tournaments
- Tournament Applications
- Tournament Participants
- Tournament Results
- Sponsorship Packages
- Sponsorship Requests
- Shortlisted Athletes
- Scouting Notes
- Notifications
- Verification Requests
- Audit Logs

The database design uses primary keys, foreign keys, appropriate constraints, timestamps, and indexes to maintain data integrity and support efficient queries.

## 🔐 Security

TALORIA aims to implement appropriate security practices, including:

- Secure password storage using password hashing.
- Authentication and role-based authorization.
- Server-side input validation.
- Protection against SQL injection through parameterized queries.
- Secure handling and validation of uploaded files.
- Environment variables for sensitive configuration.
- Appropriate access restrictions for administrative functions.
- User-friendly error handling without exposing sensitive server details.

## 👥 User Roles

| Role | Responsibilities |
|---|---|
| Athlete | Creates a profile, showcases talent, and applies for tournaments. |
| Scout/Coach | Discovers, evaluates, and shortlists athletes. |
| Tournament Organizer | Creates tournaments and manages applications and participants. |
| Sponsor | Supports tournaments through sponsorship packages. |
| Administrator | Manages users, verification, and platform operations. |

## 🚀 Getting Started

The following instructions describe the general setup process. Commands and configuration may vary depending on the implemented backend and project structure.

### Prerequisites

Install the following:

- Python
- PostgreSQL
- A web browser
- A code editor such as Visual Studio Code
- Git (optional, for version control)

### Installation

#### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd TALORIA
```

Replace `<your-repository-url>` with the actual repository URL.

#### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

#### 3. Install Dependencies

If the project includes a `requirements.txt` file, run:

```bash
pip install -r requirements.txt
```

#### 4. Set Up PostgreSQL

- Start the PostgreSQL server.
- Create a database named `taloria`.
- Execute the project's SQL schema or database initialization script.
- Configure the backend with the appropriate PostgreSQL connection details.

Example database creation command:

```sql
CREATE DATABASE taloria;
```

#### 5. Configure Environment Variables

Create a `.env` file if the backend uses environment variables. Add the required database connection settings, application secrets, and other configuration values.

Example placeholders:

```env
DATABASE_URL=your_postgresql_connection_string
SECRET_KEY=your_secret_key
```

Use the variable names expected by your application. Replace the placeholders with valid values and never commit real credentials to version control.

#### 6. Start the Backend

Run the Python entry point configured in your project. For example, if the application uses `main.py`:

```bash
python main.py
```

#### 7. Open the Application

Open the frontend through the configured development server or hosting setup. Ensure the backend is running and connected to PostgreSQL before testing database-dependent features.

## 📂 Suggested Project Structure

The following is a suggested structure. The actual files should match the implemented application.

```text
TALORIA/
│
├── frontend/
│   ├── index.html
│   ├── login.html
│   ├── register.html
│   ├── athlete.html
│   ├── scout.html
│   ├── organizer.html
│   ├── sponsor.html
│   ├── admin.html
│   ├── style.css
│   └── script.js
│
├── backend/
│   ├── main.py
│   ├── database.py
│   ├── auth.py
│   ├── athlete.py
│   ├── scout.py
│   ├── tournament.py
│   ├── sponsor.py
│   └── admin.py
│
├── database/
│   └── taloria.sql
│
├── uploads/
│
├── .env.example
├── .gitignore
├── requirements.txt
└── README.md
```

## 🧪 Testing

The application should be tested for the following scenarios:

- User registration and login.
- Role-based access restrictions.
- Athlete profile creation and updates.
- Tournament creation and discovery.
- Application submission and approval or rejection.
- Duplicate applications and closed tournaments.
- Athlete search, filtering, sorting, and pagination.
- Sponsorship request submission and approval.
- Profile verification.
- Notification creation and read status.
- Database relationships and invalid inputs.
- File upload validation.
- Error handling during backend or database failures.

## 📊 Expected Benefits

- Improves visibility for talented athletes.
- Connects athletes with scouts and coaches.
- Creates more opportunities through tournament participation.
- Helps organizers manage tournament registrations.
- Enables sponsors to support sporting events.
- Provides a structured platform for discovering talent through measurable performance.

## 🔮 Future Enhancements

- Email notifications and account verification.
- Improved tournament result management.
- Advanced performance analytics.
- Additional sports and tournament categories.
- Secure messaging between athletes and scouts.
- Enhanced mobile responsiveness.
- Integration with external tournament result systems.

## 📌 Project Scope

TALORIA is built around conventional software logic, relational databases, user-provided information, and measurable performance statistics. It does **not** depend on artificial intelligence for its core talent discovery, search, filtering, or ranking functionality.

Features should be considered implemented only after they are connected to the backend and database and have been tested.

## 👨‍💻 Project Information

- **Project Name:** TALORIA
- **Domain:** Sports Technology and Talent Discovery
- **Project Type:** Full-Stack Web Application
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Python
- **Database:** PostgreSQL
- **Architecture:** Three-Tier Architecture
- **Methodology:** Agile Scrum
- **Tagline:** Where Talent Finds Its Stage.

## 📄 License

A license can be added once the project's distribution and reuse terms have been decided.
