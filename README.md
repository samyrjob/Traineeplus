<p align="center">
  <img src="https://img.shields.io/badge/Trainee+-International%20Internship%20Platform-6366f1?style=for-the-badge&labelColor=1e1e2e" alt="Trainee+ Banner"/>
</p>

<h1 align="center">🎓 Trainee+</h1>

<p align="center">
  <strong>Connecting French Grandes Écoles students with European tech startups</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=flat-square" alt="Status"/>
  <img src="https://img.shields.io/badge/Duration-July%202022%20–%20August%202023-blue?style=flat-square" alt="Duration"/>
  <img src="https://img.shields.io/badge/Type-Entrepreneurial%20Project-purple?style=flat-square" alt="Type"/>
</p>

---

## 📋 Overview

**Trainee+** is a dual-authentication web platform developed under Audencia's **Emerge entrepreneurship program**. The platform was designed to bridge the gap between French Grandes Écoles students seeking international internships and startups across **5 European French Tech hubs**.

---

## 🛠️ Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Ruby-CC342D?style=for-the-badge&logo=ruby&logoColor=white" alt="Ruby"/>
  <img src="https://img.shields.io/badge/Ruby_on_Rails_7-CC0000?style=for-the-badge&logo=ruby-on-rails&logoColor=white" alt="Rails"/>
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3"/>
  <img src="https://img.shields.io/badge/Heroku-430098?style=for-the-badge&logo=heroku&logoColor=white" alt="Heroku"/>
  <img src="https://img.shields.io/badge/Minitest-CC342D?style=for-the-badge&logo=ruby&logoColor=white" alt="Minitest"/>
</p>

### Integrations & Services

<p align="center">
  <img src="https://img.shields.io/badge/SendGrid-1A82E2?style=for-the-badge&logo=sendgrid&logoColor=white" alt="SendGrid"/>
  <img src="https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white" alt="Cloudinary"/>
  <img src="https://img.shields.io/badge/Devise-430098?style=for-the-badge&logo=ruby&logoColor=white" alt="Devise"/>
  <img src="https://img.shields.io/badge/ActiveRecord-CC0000?style=for-the-badge&logo=ruby-on-rails&logoColor=white" alt="ActiveRecord"/>
</p>

---

## ✨ Key Features

### 🔐 Dual Authentication System
- Separate **Devise models** for students and employers
- Role-based dashboards with tailored experiences
- Scoped controllers for security and data isolation
- Custom registration flows for each user type

### 🗄️ Robust Data Architecture
- Relational **PostgreSQL schema** with 6 interconnected models
- Application status workflows: `pending → accepted / declined / kept`
- Multi-criteria search engine using **SQL ILIKE** for fuzzy matching
- Search across jobs, companies, and locations

### 📧 Automated Communications
- **SendGrid API** integration for application notifications
- PDF attachment support for application documents
- Real-time status update emails

### 📁 File Management & SEO
- **Cloudinary** integration for secure file storage
- **FriendlyId** for SEO-friendly, human-readable URLs
- **Action Text** for rich job description formatting

---

## 📊 Impact & Results

<table>
  <tr>
    <td align="center">
      <h3>👨‍🎓 130</h3>
      <p>Students Served</p>
    </td>
    <td align="center">
      <h3>🏢 16</h3>
      <p>Partner Startups</p>
    </td>
    <td align="center">
      <h3>🌍 5</h3>
      <p>European Tech Hubs</p>
    </td>
  </tr>
</table>

### Achievements

- ✅ **Simplified internship access** for 130 students by reducing search time and increasing match relevance
- ✅ **Connected 16 startups** with qualified, pre-screened candidates from top French business schools
- ✅ **Strengthened cross-border recruitment** for French startups across 5 European French Tech hubs

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                      Trainee+ Platform                       │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ┌─────────────┐          ┌─────────────┐                  │
│  │   Student   │          │   Employer  │                  │
│  │  Dashboard  │          │  Dashboard  │                  │
│  └──────┬──────┘          └──────┬──────┘                  │
│         │                        │                          │
│         └────────────┬───────────┘                          │
│                      │                                      │
│              ┌───────▼───────┐                              │
│              │  Devise Auth  │                              │
│              │  (Dual Model) │                              │
│              └───────┬───────┘                              │
│                      │                                      │
│    ┌─────────────────┼─────────────────┐                   │
│    │                 │                 │                    │
│    ▼                 ▼                 ▼                    │
│ ┌──────┐       ┌──────────┐      ┌──────────┐             │
│ │ Jobs │◄─────►│ Companies│◄────►│Applications│            │
│ └──────┘       └──────────┘      └──────────┘             │
│                                                             │
├─────────────────────────────────────────────────────────────┤
│  PostgreSQL  │  SendGrid  │  Cloudinary  │  Heroku         │
└─────────────────────────────────────────────────────────────┘
```

---

## 🚀 Getting Started

### Prerequisites

- ![Ruby](https://img.shields.io/badge/Ruby-3.x-CC342D?style=flat-square&logo=ruby&logoColor=white)
- ![Rails](https://img.shields.io/badge/Rails-7.x-CC0000?style=flat-square&logo=ruby-on-rails&logoColor=white)
- ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-14+-316192?style=flat-square&logo=postgresql&logoColor=white)

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/trainee-plus.git
cd trainee-plus

# Install dependencies
bundle install

# Setup database
rails db:create db:migrate db:seed

# Start the server
rails server
```

### Environment Variables

```bash
# .env
SENDGRID_API_KEY=your_sendgrid_key
CLOUDINARY_URL=your_cloudinary_url
DATABASE_URL=your_postgres_url
```

---

## 📁 Project Structure

```
trainee-plus/
├── app/
│   ├── controllers/
│   │   ├── students/          # Student-scoped controllers
│   │   └── employers/         # Employer-scoped controllers
│   ├── models/
│   │   ├── student.rb         # Student Devise model
│   │   ├── employer.rb        # Employer Devise model
│   │   ├── job.rb
│   │   ├── company.rb
│   │   ├── application.rb
│   │   └── ...
│   └── views/
├── config/
├── db/
│   └── schema.rb              # 6 interconnected models
└── test/                      # Minitest test suite
```

---

## 📄 License

This project was developed as part of an entrepreneurial initiative under Audencia's Emerge program.

---

<p align="center">
  <strong>Built with ❤️ for the French Tech ecosystem</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-Ruby%20on%20Rails-CC0000?style=flat-square&logo=ruby-on-rails" alt="Made with Rails"/>
</p>
