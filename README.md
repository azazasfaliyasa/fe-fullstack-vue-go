# Fullstack User Management - Frontend (Vue.js)

Frontend untuk aplikasi **User Management** fullstack menggunakan **Vue.js 3 + TypeScript**.  
Aplikasi ini berfungsi untuk **autentikasi pengguna**, **registrasi**, serta **CRUD user management** melalui integrasi API backend (Go).

---

## 🚀 Features
- Login & Register dengan JWT Authentication
- Protected routes (hanya user yang login bisa akses)
- CRUD user (Create, Read, Update, Delete)
- **TanStack Query (Vue Query)** untuk data fetching & caching
- **CORS** enabled (akses API dari backend Go)
- Routing terstruktur dengan Vue Router
- Responsive UI dengan Tailwind CSS

---

## 🛠️ Tech Stack
- **Framework**: Vue.js 3 + TypeScript
- **Routing**: Vue Router
- **State/Data**: TanStack Query (Vue Query)
- **Styling**: Tailwind CSS
- **Build Tool**: Vite
- **Auth**: JWT (dari backend Go)

---

## 📂 Project Structure
```
fe-fullstack-vue-go/
├── .gitignore
├── index.html
├── package-lock.json
├── package.json
├── public/
│   ├── vite.svg
├── README.md
├── src/
│   ├── App.vue
│   ├── assets/
│   │   ├── vue.svg
│   ├── components/
│   │   ├── HelloWorld.vue
│   │   ├── SidebarMenu.vue
│   ├── composables/
│   │   ├── auth/
│   │   │   ├── useAuthUser.ts
│   │   │   ├── useLogin.ts
│   │   │   ├── useLogout.ts
│   │   │   ├── useRegister.ts
│   │   ├── user/
│   │   │   ├── useUserById.ts
│   │   │   ├── useUserCreate.ts
│   │   │   ├── useUserDelete.ts
│   │   │   ├── useUsers.ts
│   │   │   ├── useUserUpdate.ts
│   ├── main.ts
│   ├── routes/
│   │   ├── index.ts
│   ├── services/
│   │   ├── api.ts
│   ├── shims-vue.d.ts
│   ├── style.css
│   ├── views/
│   │   ├── admin/
│   │   │   ├── dashboard/
│   │   │   │   ├── index.vue
│   │   │   ├── users/
│   │   │   │   ├── create.vue
│   │   │   │   ├── edit.vue
│   │   │   │   ├── index.vue
│   │   ├── auth/
│   │   │   ├── login.vue
│   │   │   ├── register.vue
│   │   ├── home/
│   │   │   ├── index.vue
│   ├── vite-env.d.ts
├── tsconfig.json
├── tsconfig.node.json
├── vite.config.ts
```

---

## ⚙️ Environment Variables
Buat file `.env` atau `.env.local` di root project:

```env
VITE_API_URL=http://localhost:3000
```

---

## ▶️ Running the Project
```bash
# Install dependencies
npm install

# Jalankan development server
npm run dev
```

Frontend akan berjalan di:  
👉 `http://localhost:5173`

---

## 🔗 API Integration
Semua request data menggunakan **TanStack Query**, dengan base URL diambil dari `VITE_API_URL`.  
Pastikan backend Go sudah berjalan di port yang sesuai (default `3000`).

---

## 📌 Pages
- `/login` → Halaman login
- `/register` → Halaman registrasi
- `/` → Home
- `/admin/dashboard` → Dashboard admin
- `/admin/users` → List user
- `/admin/users/create` → Tambah user
- `/admin/users/:id/edit` → Edit user

---

## 🤝 Contribution
Feel free to fork and submit pull requests.

---

## 📄 License
This project is licensed under the MIT License.
