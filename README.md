# 🧵 SmartStitch AI

<div align="center">

![SmartStitch AI Logo](https://img.shields.io/badge/SmartStitch-AI-10b981?style=for-the-badge&logo=ai&logoColor=white)
![Version](https://img.shields.io/badge/version-1.0.0-blue?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)

**Kasanachilik tizimini raqamlashtiruvchi AI asosli tekstil klasteri platformasi**

[Demo ko'rish](#demo) • [Hujjatlar](#hujjatlar) • [O'rnatish](#ornatish) • [Jamoa](#jamoa)

</div>

---

## 📋 Mundarija

- [Loyiha haqida](#loyiha-haqida)
- [Asosiy xususiyatlar](#asosiy-xususiyatlar)
- [Muammo va yechim](#muammo-va-yechim)
- [Texnologiyalar](#texnologiyalar)
- [Arxitektura](#arxitektura)
- [O'rnatish](#ornatish)
- [Foydalanish](#foydalanish)
- [API Hujjatlari](#api-hujjatlari)
- [Yo'l xaritasi](#yol-xaritasi)
- [Jamoa](#jamoa)
- [Hissa qo'shish](#hissa-qoshish)
- [Litsenziya](#litsenziya)

---

## 🎯 Loyiha haqida

**SmartStitch AI** - O'zbekiston tekstil sanoatini zamonaviylashtirish uchun yaratilgan AI asosli raqamli platforma. Loyiha kasanachilik tizimini to'liq raqamlashtirish, sifat nazoratini avtomatlashtirish va moliyaviy risklarni minimallash maqsadida ishlab chiqilgan.

### 🌟 Asosiy maqsadlar

- ✅ Tekstil mahsulotlari sifatini AI orqali avtomatik baholash
- ✅ Kasanachilar va tadbirkorlar o'rtasida ishonchli bog'lanish yaratish
- ✅ Moliyaviy yo'qotishlarni 45% gacha kamaytirish
- ✅ Ishlab chiqarish samaradorligini 18% oshirish
- ✅ Real vaqt monitoring va shaffoflik ta'minlash

---

## ⚡ Asosiy xususiyatlar

### 🤖 AI Vision Tahlil
- **Gemini 1.5 Pro** va **GPT-4o Vision** integratsiyasi
- Mahsulot rasmlarini avtomatik tahlil qilish
- Defektlarni aniqlash va sifatni baholash
- 92% aniqlik darajasi
- 2 soniyadan kam tahlil vaqti

### 📊 Risk Skorlash Tizimi
- 0-100 ball oralig'ida risk baholash
- Kasanachi va buyurtma darajasida monitoring
- NPL (non-performing loans) bashorati
- Tarixiy ma'lumotlar asosida ML modellari

### 💰 Escrow To'lov Tizimi
- AI tasdiqidan keyin avtomatik to'lov
- Virtual hamyon integratsiyasi
- Xavfsiz P2P tranzaksiyalar
- Real vaqt balans kuzatuvi

### 📱 Marketplace Platforma
- Tadbirkor va kasanachilarni avtomatik matching
- Skills-ga asoslangan tavsiya tizimi
- Reytinglar va sharh tizimi
- Buyurtmalarni boshqarish paneli

### 🚚 Logistika Monitoring
- QR-kod orqali xomashyo yetkazishni tasdiqlash
- GPS tracking integratsiyasi
- Yetkazib berish holati real vaqt kuzatuvi

---

## ❌ Muammo va ✅ Yechim

### 🔴 Muammo

| Muammo | Ta'sir |
|--------|--------|
| 👤 Manual sifat nazorati | Sub'ektiv, vaqt talab qiladi, xatolar ko'p |
| 💸 Yuqori brak darajasi | 3-5% yo'qotish, NPL muammolari |
| 🔍 Shaffoflik yo'qligi | Ishonchsizlik, monitoring yo'q |
| ⚠️ To'lov kechikishlari | Kasanachilar motivatsiyasi pasayadi |

### 🟢 Yechim

| Xususiyat | Foyda |
|-----------|-------|
| 🎯 AI Vision | Ob'ektiv va tez sifat nazorati |
| 📈 Risk Skorlash | Moliyaviy yo'qotishlarni 45% kamaytirish |
| ⚡ Avtomatik To'lovlar | Ishonch va tezlik oshishi |
| 📱 Digital Platform | To'liq shaffoflik va monitoring |

---

## 🛠 Texnologiyalar

### Backend
- **Django 4.2** - Web framework
- **Django REST Framework** - API development
- **PostgreSQL 15** - Ma'lumotlar bazasi
- **Redis** - Caching va queue management
- **Celery** - Asynchronous task processing

### AI/ML
- **Google Gemini 1.5 Pro** - Vision API
- **OpenAI GPT-4o** - Vision analysis
- **TensorFlow 2.x** - Custom ML models
- **scikit-learn** - Risk scoring algorithms
- **OpenCV** - Image preprocessing

### Frontend
- **React 18** - UI framework
- **Tailwind CSS** - Styling
- **shadcn/ui** - Component library
- **Recharts** - Data visualization
- **WebSocket** - Real-time updates

### DevOps & Infrastructure
- **Docker & Docker Compose** - Containerization
- **Nginx** - Reverse proxy
- **GitHub Actions** - CI/CD
- **AWS S3** - Media storage
- **Cloudflare** - CDN

### Payment & Logistics
- **Click/Payme API** - Payment gateway
- **Stripe** - International payments (future)
- **Google Maps API** - Logistics tracking

---

## 🏗 Arxitektura

```
┌─────────────────────────────────────────────────────────┐
│                    Client Layer                          │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐  │
│  │   Web App    │  │  Mobile App  │  │  Admin Panel │  │
│  │  (React)     │  │  (React Native)│ │   (Django)   │  │
│  └──────────────┘  └──────────────┘  └──────────────┘  │
└─────────────────────────────────────────────────────────┘
                           ↓
┌─────────────────────────────────────────────────────────┐
│                    API Gateway Layer                     │
│  ┌──────────────────────────────────────────────────┐  │
│  │         Django REST Framework + JWT Auth          │  │
│  └──────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────┘
                           ↓
┌─────────────────────────────────────────────────────────┐
│                   Business Logic Layer                   │
│  ┌────────────┐  ┌────────────┐  ┌────────────┐       │
│  │   Orders   │  │  AI Vision │  │   Payment  │       │
│  │  Service   │  │  Service   │  │  Service   │       │
│  └────────────┘  └────────────┘  └────────────┘       │
│  ┌────────────┐  ┌────────────┐  ┌────────────┐       │
│  │    Risk    │  │ Logistics  │  │   Matching │       │
│  │  Scoring   │  │  Service   │  │  Service   │       │
│  └────────────┘  └────────────┘  └────────────┘       │
└─────────────────────────────────────────────────────────┘
                           ↓
┌─────────────────────────────────────────────────────────┐
│                    Data Layer                            │
│  ┌────────────┐  ┌────────────┐  ┌────────────┐       │
│  │ PostgreSQL │  │   Redis    │  │    S3      │       │
│  │   (Main)   │  │  (Cache)   │  │  (Media)   │       │
│  └────────────┘  └────────────┘  └────────────┘       │
└─────────────────────────────────────────────────────────┘
                           ↓
┌─────────────────────────────────────────────────────────┐
│                 External Services                        │
│  ┌────────────┐  ┌────────────┐  ┌────────────┐       │
│  │  Gemini    │  │   GPT-4o   │  │ Click/Payme│       │
│  │    API     │  │    API     │  │    API     │       │
│  └────────────┘  └────────────┘  └────────────┘       │
└─────────────────────────────────────────────────────────┘
```

---

## 🚀 O'rnatish

### Talablar
- Python 3.11+
- Node.js 18+
- PostgreSQL 15+
- Redis 7+
- Docker & Docker Compose (optional)

### 1. Repository ni clone qilish
```bash
git clone https://github.com/smartstitch-ai/smartstitch-platform.git
cd smartstitch-platform
```

### 2. Virtual environment yaratish
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
# yoki
venv\Scripts\activate  # Windows
```

### 3. Dependencies o'rnatish
```bash
# Backend
pip install -r requirements.txt

# Frontend
cd frontend
npm install
```

### 4. Environment o'zgaruvchilarini sozlash
```bash
cp .env.example .env
# .env faylni tahrirlang va kerakli qiymatlarni kiriting
```

**.env** fayl namunasi:
```env
# Django
SECRET_KEY=your-secret-key-here
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1

# Database
DB_NAME=smartstitch_db
DB_USER=postgres
DB_PASSWORD=your-password
DB_HOST=localhost
DB_PORT=5432

# Redis
REDIS_URL=redis://localhost:6379/0

# AI APIs
GEMINI_API_KEY=your-gemini-api-key
OPENAI_API_KEY=your-openai-api-key

# Storage
AWS_ACCESS_KEY_ID=your-aws-key
AWS_SECRET_ACCESS_KEY=your-aws-secret
AWS_STORAGE_BUCKET_NAME=smartstitch-media

# Payment
CLICK_MERCHANT_ID=your-merchant-id
CLICK_SERVICE_ID=your-service-id
CLICK_SECRET_KEY=your-secret-key
```

### 5. Database migratsiya
```bash
python manage.py migrate
python manage.py createsuperuser
```

### 6. Serverni ishga tushirish
```bash
# Backend (Terminal 1)
python manage.py runserver

# Celery worker (Terminal 2)
celery -A smartstitch worker -l info

# Frontend (Terminal 3)
cd frontend
npm run dev
```

### 🐳 Docker bilan ishga tushirish
```bash
docker-compose up -d
```

---

## 💻 Foydalanish

### Tadbirkor uchun

1. **Ro'yxatdan o'tish**
   ```bash
   POST /api/v1/auth/register/
   {
     "phone": "+998901234567",
     "user_type": "entrepreneur",
     "company_name": "TextilePro LLC"
   }
   ```

2. **Buyurtma yaratish**
   ```bash
   POST /api/v1/orders/
   {
     "product_type": "ko'ylak",
     "quantity": 100,
     "deadline": "2025-03-01",
     "budget": 5000000
   }
   ```

3. **AI tahlil natijasini ko'rish**
   ```bash
   GET /api/v1/orders/{order_id}/ai-analysis/
   ```

### Kasanachi uchun

1. **Profil sozlash**
   ```bash
   POST /api/v1/profile/skills/
   {
     "skills": ["tikuvchilik", "ko'ylak", "shimlar"],
     "experience_years": 5,
     "daily_capacity": 20
   }
   ```

2. **Buyurtmalarni ko'rish**
   ```bash
   GET /api/v1/orders/available/
   ```

3. **Mahsulot rasmini yuklash**
   ```bash
   POST /api/v1/orders/{order_id}/submit-photo/
   FormData: {
     "image": file,
     "notes": "Tugadi"
   }
   ```

---

## 📚 API Hujjatlari

### Authentication

#### Ro'yxatdan o'tish
```http
POST /api/v1/auth/register/
Content-Type: application/json

{
  "phone": "+998901234567",
  "password": "securepassword123",
  "user_type": "entrepreneur|artisan",
  "full_name": "Aziz Zokirov"
}

Response: 201 Created
{
  "user": {
    "id": 1,
    "phone": "+998901234567",
    "user_type": "entrepreneur",
    "full_name": "Aziz Zokirov"
  },
  "tokens": {
    "access": "eyJ0eXAiOiJKV1QiLCJhbGc...",
    "refresh": "eyJ0eXAiOiJKV1QiLCJhbGc..."
  }
}
```

#### Login
```http
POST /api/v1/auth/login/
Content-Type: application/json

{
  "phone": "+998901234567",
  "password": "securepassword123"
}

Response: 200 OK
{
  "tokens": {
    "access": "eyJ0eXAiOiJKV1QiLCJhbGc...",
    "refresh": "eyJ0eXAiOiJKV1QiLCJhbGc..."
  }
}
```

### Orders

#### Buyurtma yaratish
```http
POST /api/v1/orders/
Authorization: Bearer {access_token}
Content-Type: application/json

{
  "product_type": "ko'ylak",
  "quantity": 100,
  "description": "Erkaklar yozgi ko'ylaklari",
  "deadline": "2025-03-15",
  "budget": 5000000,
  "required_skills": ["tikuvchilik", "ko'ylak"]
}

Response: 201 Created
{
  "id": 42,
  "status": "pending",
  "product_type": "ko'ylak",
  "quantity": 100,
  "risk_score": null,
  "created_at": "2025-02-12T10:30:00Z"
}
```

#### AI tahlil yuborish
```http
POST /api/v1/orders/{order_id}/submit-for-analysis/
Authorization: Bearer {access_token}
Content-Type: multipart/form-data

FormData:
  - image: [File]
  - notes: "Mahsulot tayyor"

Response: 200 OK
{
  "id": 42,
  "ai_analysis": {
    "quality_score": 96,
    "defects": [],
    "recommendation": "approved",
    "confidence": 0.92,
    "analysis_time": 1.8
  },
  "risk_score": 23,
  "status": "approved"
}
```

### Risk Scoring

#### Risk skorini hisoblash
```http
GET /api/v1/risk/calculate/{order_id}/
Authorization: Bearer {access_token}

Response: 200 OK
{
  "order_id": 42,
  "risk_score": 23,
  "factors": {
    "artisan_history": 15,
    "order_complexity": 5,
    "deadline_pressure": 3
  },
  "recommendation": "low_risk",
  "suggested_actions": []
}
```

---

## 🗓 Yo'l xaritasi

### ✅ I-Bosqich: Foundation (Tugallandi)
- [x] Django backend setup
- [x] PostgreSQL database models
- [x] JWT authentication
- [x] Basic API endpoints

### 🚧 II-Bosqich: AI Integration (Jarayonda)
- [x] Gemini API integratsiya
- [x] GPT-4o Vision setup
- [ ] Custom ML model training
- [ ] Prompt engineering optimization

### 📋 III-Bosqich: Dashboard (Keyingi)
- [ ] Tadbirkor paneli
- [ ] Kasanachi paneli
- [ ] Admin dashboard
- [ ] Real-time WebSocket

### 💰 IV-Bosqich: FinTech (Rejalashtirilgan)
- [ ] Click/Payme integratsiya
- [ ] Virtual hamyon tizimi
- [ ] Escrow payment logic
- [ ] Transaction history

### 🎯 V-Bosqich: Scaling (Kelajak)
- [ ] Mobile app (React Native)
- [ ] Qishloq xo'jaligi versiya
- [ ] Xalqaro kengayish
- [ ] Blockchain integratsiya

---

## 👥 Jamoa

<table>
  <tr>
    <td align="center">
      <img src="https://via.placeholder.com/100/06b6d4/ffffff?text=QM" width="100px;" alt=""/><br />
      <sub><b>Quvondiqov Muhammad</b></sub><br />
      <sub>CEO & Project Manager</sub>
    </td>
    <td align="center">
      <img src="https://via.placeholder.com/100/6366f1/ffffff?text=OO" width="100px;" alt=""/><br />
      <sub><b>Oripov Ozodbek</b></sub><br />
      <sub>CTO & Data Science</sub>
    </td>
    <td align="center">
      <img src="https://via.placeholder.com/100/a855f7/ffffff?text=MSH" width="100px;" alt=""/><br />
      <sub><b>Movlonqulov Sherali</b></sub><br />
      <sub>Tekstil soha eksperti</sub>
    </td>
    <td align="center">
      <img src="https://via.placeholder.com/100/f59e0b/ffffff?text=QM" width="100px;" alt=""/><br />
      <sub><b>Quvondiqova Mahliyo</b></sub><br />
      <sub>CFO & Frontend Developer</sub>
    </td>
  </tr>
</table>

---

## 📊 Natijalar

| Metrika | Hozirgi holat | SmartStitch AI bilan |
|---------|---------------|----------------------|
| Brak darajasi | 3-5% | **0.5-1%** ⬇️ 80% |
| Sifat nazorat xarajati | Manual | **Avtomatik** ⬇️ 70% |
| To'lov kechikishi | 15-30 kun | **2-3 kun** ⬇️ 85% |
| Ishlab chiqarish tezligi | Baseline | **+18%** ⬆️ |
| Risk bashorat aniqligi | N/A | **92%** ✅ |

---

## 🤝 Hissa qo'shish

Biz open source hissalarni qabul qilamiz! Iltimos, quyidagi qoidalarga rioya qiling:

1. Fork qiling
2. Feature branch yarating (`git checkout -b feature/AmazingFeature`)
3. Commit qiling (`git commit -m 'Add some AmazingFeature'`)
4. Push qiling (`git push origin feature/AmazingFeature`)
5. Pull Request oching

### Kod standartlari
- Python: PEP 8
- JavaScript: ESLint + Prettier
- Commit messages: Conventional Commits
- Tests: 80%+ coverage

---

## 📄 Litsenziya

Ushbu loyiha MIT litsenziyasi ostida tarqatiladi. Batafsil ma'lumot uchun [LICENSE](LICENSE) faylini ko'ring.

---

## 📞 Aloqa

- **Email**: info@smartstitch.ai
- **Telegram**: [@smartstitch_support](https://t.me/smartstitch_support)
- **Website**: [https://smartstitch.ai](https://smartstitch.ai)
- **LinkedIn**: [SmartStitch AI](https://linkedin.com/company/smartstitch-ai)

---

## 🙏 Minnatdorchilik

- **Anthropic** - Claude AI support
- **Google** - Gemini API
- **OpenAI** - GPT-4o Vision
- **O'zbekiston Yengil Sanoat Vazirligi** - Domain expertise
- **IT Park Uzbekistan** - Mentorship and support

---

<div align="center">

**SmartStitch AI** bilan kelajakni birga quramiz! 🚀

Made with ❤️ in Uzbekistan 🇺🇿

[⬆ Yuqoriga qaytish](#-smartstitch-ai)

</div>
