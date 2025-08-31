# 🐷 Smart Pig - Invisible DeFi Yield Farming WEBSITE ONLY

> **The first solution worldwide that makes yield farming as simple as PIX payments**

Smart Pig democratizes access to DeFi in Brazil through the world's first solution that makes yield farming indistinguishable from traditional savings, offering 7-10% annual returns in USDC through a gamified experience.

## 🎯 **Problem We Solve**

- 💤 **R$ 1.2 trillion** sitting idle in savings accounts earning only 6% p.a.
- 🌐 Only **3% of population** accesses DeFi due to technical complexity  
- 💱 Bank spreads of **4-6%** make dollar protection expensive for most Brazilians
- 🔒 **86% of Brazilians** want alternatives to traditional savings

## ⚡ **Our Solution**

**Invisible DeFi**: PIX (R$) → Smart Pig → Aquarius Pools → 7-10% p.a. USDC


## 🛠️ **Tech Stack**

### Frontend
- **HTML5** + **CSS3** + **Vanilla JavaScript**
- **Responsive Design** (Mobile-first)
- **Custom Animations** (bounce, glow, float)
- **Progressive Enhancement**

### Backend & Database  
- **Supabase** (PostgreSQL + Real-time API)
- **Row Level Security (RLS)**
- **UTM Tracking** for marketing analytics

### Deployment
- **Netlify** (Global CDN, Auto HTTPS, Continuous Deployment)
- **GitHub Actions** (CI/CD pipeline)

## 🏗️ **Project Structure**

```
📁 SmartPig-website/
├── 📄 index.html          # Main landing page
├── 🖼️ smart-pig.svg       # Custom pig mascot
├── 📋 README.md           # Project documentation
└── 📝 .gitignore          # Git ignore rules
```

## 🚀 **Getting Started**

### Prerequisites
- Modern web browser
- Git installed
- Supabase account (for backend)

### Local Development

1. **Clone the repository**
```bash
git clone https://github.com/CarolTea/SmartPig-website.git
cd SmartPig-website
```

2. **Open in browser**
```bash
# Simply open index.html in your browser
# Or use a local server (recommended):
python -m http.server 8000
# Then visit: http://localhost:8000
```

3. **Configure Supabase** (Optional for development)
- Create project at [supabase.com](https://supabase.com)
- Update credentials in `index.html`
- Run SQL to create `early_adopters` table

## 🗄️ **Database Schema**

```sql
CREATE TABLE early_adopters (
  id UUID DEFAULT gen_random_uuid() PRIMARY KEY,
  name VARCHAR(255) NOT NULL,
  email VARCHAR(255) UNIQUE NOT NULL,
  phone VARCHAR(20),
  created_at TIMESTAMP WITH TIME ZONE DEFAULT NOW(),
  utm_source VARCHAR(50) DEFAULT 'website',
  utm_campaign VARCHAR(50) DEFAULT 'early-adopter'
);
```

## 📈 **Analytics & Tracking**

The website includes built-in UTM parameter tracking:

- `utm_source`: Traffic source (google, facebook, instagram, etc.)
- `utm_campaign`: Campaign name (early-adopter, launch, ads, etc.)

**Example URLs:**
- Direct: `smartpig.com`
- Instagram: `smartpig.com?utm_source=instagram&utm_campaign=launch`
- Google Ads: `smartpig.com?utm_source=google&utm_campaign=ads`

## 🛡️ **Security Features**

- ✅ **Biometric Authentication** (Passkeys - Face ID/Touch ID/Windows Hello)
- ✅ **Row Level Security** in Supabase
- ✅ **Input Validation** and sanitization
- ✅ **HTTPS Everywhere** (Netlify auto-SSL)
- ✅ **Content Security Policy** headers
- ✅ **XSS Protection** built-in

## 🎨 **Design System**

### Color Palette
- **Primary Gold**: `#FFD700` (trust and confidence)  
- **Vibrant Yellow**: `#FFEB3B` (energy and optimism)
- **Neon Green**: `#C6FF00` (technology and growth)
- **Pig Accent**: `#FF8A65` (warm salmon for mascot)
- **Background**: `linear-gradient(135deg, #1a1a1a 0%, #2A5298 100%)`

### Visual Style
- Dark theme with glowing accents
- Smooth animations (bounce, glow, progress bars)
- Mobile-first responsive design
- Gamification elements

## 📱 **Responsive Design**

The website is fully responsive and optimized for:
- 📱 Mobile devices (320px+)
- 📟 Tablets (768px+)  
- 💻 Desktop (1024px+)
- 🖥️ Large screens (1440px+)

## 🚀 **Deployment**

### Automatic Deployment (Recommended)
Every push to `main` branch automatically deploys to Netlify.

### Manual Deployment
1. Build the project (if needed)
2. Deploy to Netlify via drag-and-drop or CLI
3. Configure custom domain (optional)

## 🤝 **Contributing**

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 **License**

This project is proprietary and confidential. All rights reserved.

## 📞 **Contact**


---

**Made with ❤️ in Brazil**

🐷 *"Transforming complex DeFi into something as simple as using PIX"*