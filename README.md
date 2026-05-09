# 🎯 Trần Hồng Sơn — Marketing Portfolio

Website portfolio cá nhân được xây dựng với Node.js + Express + EJS.

## 🚀 Cài đặt & Chạy local

```bash
# 1. Clone repo
git clone <your-repo-url>
cd portfolio

# 2. Cài dependencies
npm install

# 3. Chạy server
npm start

# Mở http://localhost:3000
```

## 📁 Cấu trúc thư mục

```
portfolio/
├── public/
│   ├── css/
│   │   └── style.css           # Toàn bộ CSS
│   ├── js/
│   │   └── main.js             # JavaScript
│   ├── files/
│   │   └── CV_Tran_Hong_Son.pdf  # File CV để tải
│   └── images/
│       ├── avatar/
│       │   └── avatar.jpg        # Ảnh đại diện
│       ├── software/             # Logo phần mềm (svg/png)
│       │   ├── photoshop.svg
│       │   ├── premiere.svg
│       │   ├── illustrator.svg
│       │   ├── aftereffects.svg
│       │   ├── canva.svg
│       │   ├── chatgpt.svg
│       │   ├── midjourney.svg
│       │   └── wordpress.svg
│       └── projects/
│           ├── brand/            # Ảnh dự án Thương hiệu
│           │   ├── brand-01.jpg
│           │   └── brand-02.jpg
│           ├── performance/      # Ảnh dự án Performance Ads
│           │   ├── perf-01.jpg
│           │   └── perf-02.jpg
│           ├── design/           # Ảnh dự án Design
│           │   ├── design-01.jpg
│           │   └── design-02.jpg
│           └── video/            # Ảnh thumbnail Video
│               ├── video-01.jpg
│               └── video-02.jpg
├── views/
│   └── index.ejs               # Template HTML chính
├── server.js                   # Express server
├── vercel.json                 # Cấu hình Vercel
├── package.json
└── .gitignore
```

## 🖼️ Cách thêm ảnh dự án

Mỗi dự án cần 1 ảnh thumbnail. Đặt ảnh vào đúng thư mục:

- **Thương hiệu**: `public/images/projects/brand/brand-01.jpg`, `brand-02.jpg`
- **Performance**: `public/images/projects/performance/perf-01.jpg`, `perf-02.jpg`
- **Design**: `public/images/projects/design/design-01.jpg`, `design-02.jpg`
- **Video**: `public/images/projects/video/video-01.jpg`, `video-02.jpg`

Để thêm dự án mới, copy 1 block `<div class="project-card">` trong `views/index.ejs` và đổi tên file ảnh, tiêu đề, mô tả.

## 🖼️ Logo phần mềm

Tải SVG logo các phần mềm và đặt vào `public/images/software/`:
- Photoshop, Premiere, Illustrator, After Effects → tải từ Adobe Press Kit
- Canva → tải từ Canva Brand assets
- ChatGPT → tải từ OpenAI Brand
- Midjourney, WordPress → tìm trên Wikimedia Commons

> Nếu không có ảnh, trang web sẽ tự hiển thị chữ viết tắt thay thế (Ps, Pr, Ai...).

## ☁️ Deploy lên Vercel

### Bước 1: Push lên GitHub
```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/<username>/<repo-name>.git
git push -u origin main
```

### Bước 2: Deploy Vercel
1. Vào [vercel.com](https://vercel.com) → Đăng nhập bằng GitHub
2. Nhấn **"Add New Project"** → Import repo vừa tạo
3. Giữ nguyên cài đặt → Nhấn **"Deploy"**
4. Vercel sẽ tự động deploy và cấp domain dạng `<tên>.vercel.app`

### Deploy tự động
Mỗi lần bạn `git push`, Vercel sẽ tự động cập nhật website.

## ✏️ Tùy chỉnh nội dung

Tất cả nội dung nằm trong `views/index.ejs`. Bạn có thể:
- Sửa thông tin liên hệ
- Thêm/xóa dự án
- Thay đổi mô tả kỹ năng
- Cập nhật kinh nghiệm làm việc

## 📱 Tính năng

- ✅ Responsive hoàn toàn (Desktop, Tablet, Mobile)
- ✅ Custom cursor với hiệu ứng follow
- ✅ Scroll reveal animations
- ✅ Skill bar animation
- ✅ Stat counter animation
- ✅ Project filter tabs
- ✅ Card hover tilt effect
- ✅ Nút tải CV
- ✅ Typing effect
- ✅ Parallax blobs
- ✅ Google Fonts tiếng Việt (Be Vietnam Pro + Playfair Display)
- ✅ Dark theme với màu đỏ chủ đạo
