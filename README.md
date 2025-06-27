# Trimrr URL Shortener

A modern, full-featured URL shortener web app. Shorten long links, customize your short URLs, generate QR codes, and track analytics (clicks, geolocation, device type) for each link. Built with React, Vite, Supabase, and Tailwind CSS.

---

## ✨ Features

- **Shorten URLs:** Instantly generate short links for any long URL.
- **Custom Aliases:** Personalize your short URLs with custom endings.
- **QR Code Generation:** Each short link comes with a downloadable QR code.
- **User Authentication:** Secure signup/login with Supabase Auth.
- **Dashboard:** Manage all your links in one place.
- **Analytics:** View total clicks, device type (mobile/desktop), and geolocation stats for each link.
- **Modern UI:** Responsive, accessible, and beautiful interface using Tailwind CSS and Radix UI.

---

## 🛠️ Tech Stack

- **Frontend:** React 18, Vite, React Router, Tailwind CSS, Radix UI
- **Backend/DB:** Supabase (Auth, Database, Storage)
- **QR Codes:** [react-qrcode-logo](https://github.com/gcoro/react-qrcode-logo)
- **Charts:** [Recharts](https://recharts.org/)
- **Validation:** Yup

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone <repo-url>
cd url-shortner
```

### 2. Install dependencies

```bash
yarn install
# or
npm install
```

### 3. Set up environment variables

Create a `.env` file in the root with the following:

```env
VITE_SUPABASE_URL=your-supabase-url
VITE_SUPABASE_KEY=your-supabase-anon-key
```

Get these values from your [Supabase project dashboard](https://app.supabase.com/).

### 4. Start the development server

```bash
yarn dev
# or
npm run dev
```

The app will be available at [http://localhost:5173](http://localhost:5173) (default Vite port).

---

## 📦 Project Structure

```
url-shortner/
├── public/                # Static assets (images, icons)
├── src/
│   ├── components/        # Reusable UI and feature components
│   ├── db/                # Supabase API wrappers (auth, urls, clicks)
│   ├── hooks/             # Custom React hooks
│   ├── layouts/           # Layout components
│   ├── lib/               # Utility functions
│   ├── pages/             # Route-based pages (landing, dashboard, link, auth)
│   ├── context.jsx        # Global context/provider
│   └── main.jsx           # App entry point
├── index.html             # Main HTML file
├── package.json           # Project metadata and scripts
├── tailwind.config.js     # Tailwind CSS config
├── vite.config.js         # Vite config
└── README.md              # Project documentation
```

---

## ⚙️ Available Scripts

- `yarn dev` / `npm run dev` — Start development server
- `yarn build` / `npm run build` — Build for production
- `yarn preview` / `npm run preview` — Preview production build
- `yarn lint` / `npm run lint` — Lint code with ESLint

---

## 🌐 Deployment

- The app is ready to deploy on any static hosting (Vercel, Netlify, etc.).
- Make sure to set the required environment variables in your hosting provider.
- Supabase handles authentication, database, and storage in the cloud.

---

## 🔒 Environment Variables

| Variable            | Description                |
|---------------------|----------------------------|
| VITE_SUPABASE_URL   | Your Supabase project URL  |
| VITE_SUPABASE_KEY   | Supabase anon/public key   |

---

## 👤 Authentication

- Users must sign up and log in to create/manage links and view analytics.
- Auth is handled via Supabase Auth (email/password).
- Profile pictures are uploaded to Supabase Storage.

---

## 📊 Analytics

- Each short link tracks:
  - Total clicks
  - Device type (mobile/desktop)
  - Geolocation (city, country)
- Analytics are displayed on the link details page.

---

## 🧩 Customization & Extensibility

- Built with modular React components and hooks.
- Easily extend with new features (e.g., more analytics, custom domains).
- Theming via Tailwind CSS.

---

## 🤝 Contributing

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

[MIT](LICENSE)

---

## 📬 Contact

- **Author:** [Your Name]
- **Email:** your.email@example.com
- **Project Link:** [GitHub Repo](<repo-url>)

---

> _Made with ❤️ using React, Vite, Supabase, and Tailwind CSS._ 
