# Fullstack User Management - Frontend (Vue.js)

Frontend for **User Management** fullstack application built with **Vue.js 3 + TypeScript**.  
This app provides **user authentication**, **registration**, and **CRUD user management** integrated with a Go backend API.

---

## 🚀 Features
- Login & Register with JWT Authentication
- Protected routes (accessible only for authenticated users)
- CRUD user (Create, Read, Update, Delete)
- **TanStack Query (Vue Query)** for data fetching & caching
- **CORS** enabled (access API from Go backend)
- Structured routing with Vue Router
- Responsive UI with Tailwind CSS

---

## 🛠️ Tech Stack
- **Framework**: Vue.js 3 + TypeScript
- **Routing**: Vue Router
- **State/Data**: TanStack Query (Vue Query)
- **Styling**: Tailwind CSS
- **Build Tool**: Vite
- **Auth**: JWT (from Go backend)

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
Create a `.env` or `.env.local` file in the project root:

```env
VITE_API_URL=http://localhost:3000
```

---

## ▶️ Running the Project
```bash
# Install dependencies
npm install

# Run development server
npm run dev
```

Frontend will be available at:  
👉 `http://localhost:5173`

---

## 🔗 API Integration
All data requests use TanStack Query, with the base URL defined by VITE_API_URL.
Make sure the Go backend is running on the matching port (default: 3000).

---

## 📌 Pages
- `/login` → Login page
- `/register` → Registration page
- `/` → Home
- `/admin/dashboard` → Admin dashboard
- `/admin/users` → User list
- `/admin/users/create` → Create new user
- `/admin/users/:id/edit` → Edit user

---

## 🤝 Contribution
Feel free to fork and submit pull requests.

---

## 📄 License
This project is licensed under the MIT License.
