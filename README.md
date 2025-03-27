# 🔥 Tinder Clone – Fullstack Dating App

Tinder Clone is a modern fullstack dating application built with **Angular** and **Spring Boot**, offering essential features like profile swiping, real-time messaging (upcoming), and intelligent match-making.

> This project replicates the core mechanics of Tinder while being fully open-source and customizable.

---

## ⚙️ Tech Stack

- **Frontend:** Angular 17+, RxJS, Angular Material / Bootstrap
- **Backend:** Java 17, Spring Boot, Spring Data JPA, Lombok
- **Database:** MySQL / PostgreSQL *(your choice)*
- **Build Tools:** Maven, Node.js, npm
- **Testing:** JUnit, Mockito, MockMvc

---

## 🚀 Key Features

### 🔐 User Authentication *(Coming Soon)*

- Secure login & registration
- JWT-based authentication
- Role-based access control (user/admin)

### 👤 Profile Management

- Create and update user profiles
- Set name, age, gender, bio, location, and profile pictures

### 💘 Swiping & Matching Logic

- Like / Dislike user profiles
- Automatic match generation when both users like each other
- Match listing per user

### 💬 Messaging *(Coming Soon)*

- Real-time chat (WebSocket or Firebase Integration)
- Match-specific chat threads
- Message history

---

## 🗂️ Project Structure

```
tinder-clone/
├── backend/              # Spring Boot application
│   ├── model             # JPA entities (User, Profile, Match, Message)
│   ├── repository        # Spring Data Repositories
│   ├── service           # Business logic
│   ├── controller        # REST API
│   ├── config            # Configuration files (security, CORS, etc.)
│   └── resources         # application.yml / properties
├── frontend/             # Angular application
│   ├── src/
│   │   ├── app/
│   │   │   ├── modules/  # Feature modules (auth, profile, match, chat)
│   │   │   ├── core/     # Shared services
│   │   │   └── shared/   # Reusable components
│   └── angular.json      # Angular project config
├── README.md
└── docs/                 # Project documentation
```

---

## 🎯 API Endpoints (Backend)

| Endpoint                 | Method | Description                       |
|--------------------------|--------|-----------------------------------|
| `/user/add`              | POST   | Register new user                 |
| `/user/findbyid/{id}`    | GET    | Get user by ID                    |
| `/user/update/{id}`      | PUT    | Update user                       |
| `/like/addlike`          | POST   | Like or dislike a user            |
| `/match/add`             | POST   | Create match if mutual likes      |
| `/messages/send`         | POST   | Send message to matched user      |
| `/messages/allbymatch/{id}` | GET  | Get all messages in a match       |

---

## 🧠 Future Additions

- ✅ JWT Auth + Spring Security  
- ✅ WebSocket chat  
- ✅ Admin dashboard  
- ✅ Notifications (with Firebase Cloud Messaging or similar)  
- ✅ Image upload with Firebase or Cloudinary  
- ✅ AI-based Match Recommendation

---

## 📌 Local Setup

### Clone the project

```bash
git clone https://github.com/your-username/tinder-clone.git
cd tinder-clone
```

### Setup Backend (Spring Boot)

```bash
cd backend
./mvnw spring-boot:run
```

- Configure DB in `application.properties` or `application.yml`
- MySQL/PostgreSQL required

### Setup Frontend (Angular)

```bash
cd frontend
npm install
ng serve
```

> Frontend runs at `http://localhost:4200`, backend at `http://localhost:8080`

---

## 💡 Contributing

Contributions are welcome! If you want to fix a bug, add a feature, or improve the code, just:

1. Fork the repo
2. Create a new branch
3. Commit your changes
4. Open a Pull Request 🚀

---

## 👨‍💻 Author

Built with ❤️ by a passionate fullstack dev on a mission to create clean and modern fullstack web apps.
