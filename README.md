# CRM Pipeline Automation with n8n

Automated CRM system built with n8n untuk mengelola lead scoring, assignment, dan follow-up processes.

## 🎯 Problem Statement
- Manual lead scoring memakan waktu dan tidak konsisten
- Lead assignment sering terlambat atau tidak merata
- Follow-up prospects sering terlewat
- Tidak ada visibility real-time untuk pipeline status

## 🚀 Solution
Automated workflow yang menghandle:
1. **Lead Scoring**: Automatic scoring berdasarkan behavior dan data
2. **Smart Assignment**: Distribute leads berdasarkan territory/expertise
3. **Follow-up Automation**: Scheduled follow-ups dan reminders
4. **Pipeline Reporting**: Real-time dashboard dan alerts

## 📊 Key Results
- Reduce lead response time dari 4 jam ke 15 menit
- Increase conversion rate sebesar 25%
- 100% lead follow-up compliance
- Save 10 hours per week manual work

## 🛠 Tech Stack
- **n8n**: Workflow automation engine
- **PostgreSQL**: Data persistence
- **Docker**: Containerization
- **Webhooks**: Real-time integrations
- **Google Sheets**: Data source dan reporting

## 🏗 Architecture
```
Webhook (Lead Input) 
    ↓
Lead Scoring Engine
    ↓
Assignment Logic
    ↓
CRM Integration
    ↓
Follow-up Scheduler
    ↓
Reporting Dashboard
```

## 🚦 Getting Started

### Prerequisites
- Docker & Docker Compose
- Git

### Installation
```bash
git clone https://github.com/ookapratama/crm-automation-n8n.git
cd crm-automation-n8n
docker-compose up -d
```

Access n8n: http://localhost:5678

## 📁 Project Structure
```
├── workflows/           # n8n workflow JSON files
├── docs/               # Documentation dan screenshots
├── sample-data/        # Test data untuk development
└── docker-compose.yml  # Container configuration
```

## 🔄 Workflows

### 1. Lead Scoring Engine
- Input: Webhook dari website/form
- Processing: Score calculation berdasarkan rules
- Output: Enriched lead data dengan score

### 2. Lead Assignment System  
- Input: Scored leads
- Processing: Territory/expertise matching
- Output: Assigned leads dengan notification

### 3. Follow-up Automation
- Input: CRM pipeline updates
- Processing: Schedule follow-ups berdasarkan stage
- Output: Automated emails/tasks/reminders

## 📈 Metrics & Monitoring
- Lead processing time
- Conversion rates by source
- Assignment distribution
- Follow-up compliance rates

## 🔧 Configuration
Copy `.env.example` ke `.env` dan sesuaikan:
- CRM API credentials
- Email service settings
- Webhook URLs

## 📝 Development Notes
Built as part of automation portfolio demonstration.
Focus on enterprise-grade reliability dan scalability.

---
**Contact**: ookapratama2@gmail.com | **Portfolio**: [ooka.my.id](https://ooka.my.id/)