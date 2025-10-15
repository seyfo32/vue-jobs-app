# Vue Jobs App

This project is a complete **Job Listings Platform** built using **Vue.js** and the **Composition API**.

It provides a realistic hands-on learning experience for building CRUD applications with Vue, working with JSON Server as a mock backend, and managing frontend routing and state.

---

## 📦 Features

- View all job listings
- View job detail pages (dynamic route)
- Create a new job listing
- Edit an existing job listing
- Delete a job listing (with confirmation prompt)
- Toast notifications for user feedback (success/error)
- API proxy setup for clean axios requests
- Loading spinners during data fetches
- Organized folder structure and reusable components
- Responsive Tailwind CSS layout

---

## 🔧 Project Setup

```bash
git clone https://github.com/seyfo32/vue-jobs-app.git
cd vue-jobs-app
npm install
```

---

## 🚀 Run the Application

In development mode:

```bash
npm run dev
```

---

## 🖥️ Run the JSON Server (Mock API)

We are using a JSON Server as a fake backend. It runs separately on port `3000` using a custom Vite config.

To start the server:

```bash
npm run server
```

This runs the following command behind the scenes:

```bash
json-server --watch jobs.json --port 3000
```

**Vite Proxy** is configured in `vite.config.js` to forward API requests (`/api`) to this mock server. This way, `axios.get('/api/jobs')` is translated to `http://localhost:3000/jobs` under the hood.

---

## 🧪 JSON Server Notes

Your mock data is stored inside `jobs.json`.

- Job entries are stored under the `jobs` array.
- On app startup, the Vue frontend makes axios requests to endpoints like `/api/jobs`, which are proxied to `http://localhost:3000/jobs`.

---

## ✨ Deployment

This app can be deployed on **Netlify**, **Vercel**, etc. However, since it uses JSON Server as backend, deployment was not done in this case.

For full deployment, a real backend API would be required.

---

## 🧠 Author

👤 **Seyfullah Bozkurt**  
💼 GitHub: [seyfo32](https://github.com/seyfo32)  
🔗 LinkedIn: [www.linkedin.com/in/seyfullah-bozkurt](https://www.linkedin.com/in/seyfullah-bozkurt)

---

## 📜 License

This project is for educational and portfolio purposes only.
