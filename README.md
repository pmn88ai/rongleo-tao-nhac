# 🎵 AI Music Studio

Một web app đơn giản giúp sáng tác bài hát bằng AI:
- Viết lời bài hát (Groq AI)
- Gợi ý giai điệu & hợp âm
- Copy sang Suno / Udio để tạo nhạc
- Lưu & quản lý bài hát ngay trên thiết bị

---

## 🚀 Demo

👉 https://your-vercel-domain.vercel.app

---

## ✨ Tính năng

### 🧠 AI sáng tác
- Tạo lời bài hát từ ý tưởng
- Viết lại / viết tiếp
- Gợi ý giai điệu (tempo, style, mood)
- Gợi ý hợp âm

---

### 🎛️ Workflow đơn giản
1. Nhập ý tưởng
2. Tạo lời
3. Gợi ý giai điệu
4. Bấm Suno / Udio
5. Dán vào → có nhạc 🎶

---

### 📋 Tiện ích
- Copy nhanh:
  - Lyrics
  - Giai điệu
  - Hợp âm
- Lưu bài hát (localStorage)
- Load / xoá bài cũ
- Export / Import JSON

---

## 🧱 Tech Stack

- Frontend: HTML + CSS + Vanilla JS
- AI: Groq API
- Deploy: Vercel
- Storage: localStorage

---

## 📦 Cấu trúc project


rongleo-tao-nhac/
├── index.html # UI + logic chính
├── api/
│ └── groq.js # API proxy (giữ key an toàn)
└── README.md


---

## ⚙️ Setup local

### 1. Clone repo

```bash
git clone https://github.com/<username>/rongleo-tao-nhac.git
cd rongleo-tao-nhac
2. Tạo file .env (local)
GROQ_API_KEY=your_key_here
3. Chạy local (Vercel dev)
npm i -g vercel
vercel dev
🚀 Deploy Vercel
1. Push code lên GitHub
git add .
git commit -m "deploy"
git push
2. Import vào Vercel
vào https://vercel.com
Add New Project
chọn repo
3. Thêm ENV
GROQ_API_KEY=your_key_here
4. Deploy 🎉
⚠️ Lưu ý quan trọng
❌ KHÔNG để API key trong frontend
❌ KHÔNG commit file .env
✅ Luôn dùng /api/groq để gọi AI
💡 Hạn chế
Không có API chính thức của Suno/Udio
→ phải copy prompt thủ công
localStorage chỉ lưu trên 1 thiết bị
🔮 Roadmap (tương lai)
 Sync cloud (Supabase)
 Auto save
 Version history
 Mobile app wrapper
 Voice input (nói ý tưởng)
👨‍🎤 Use case
Nhạc sĩ cần sketch nhanh ý tưởng
Người không biết nhạc vẫn tạo được bài
Test prompt AI music
🧠 Insight

App này không phải “AI tạo nhạc”
👉 mà là:

🎹 Công cụ hỗ trợ sáng tác cho người thật

📜 License

MIT