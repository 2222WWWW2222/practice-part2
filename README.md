# 📝 Notes Manager API (Навчальна практика з програмування. Частина 2)

Серверна частина (REST API) для системи **«Менеджер нотаток із категоріями та пошуком»**, розроблена в рамках проходження Навчальної практики з програмування (Ч.2) здобувачем освіти фаху «Комп'ютерні науки» ФПК «ОПТІМА».

---

## 🚀 Технологічний стек
- **Платформа:** Node.js
- **Фреймворк:** Express.js
- **База даних:** SQLite (`better-sqlite3`)
- **Паттерни та архітектура:** 
  - Layered Architecture (Routes → Controllers → Repositories)
  - Custom Dependency Injection (DI) Container
- **Документація:** Swagger UI (`swagger-ui-express` / OpenAPI 3.0)
- **Middleware & Логування:** Morgan, CORS, Centralized Error Handler

---

## 📊 Моделі даних (Сутності)
Застосунок працює з 3 пов'язаними сутностями:
1. **Users** (`id`, `name`, `email`)
2. **Categories** (`id`, `name`, `user_id`)
3. **Notes** (`id`, `title`, `content`, `user_id`, `category_id`)
