Sure! Here's a **cleaned-up and properly formatted** `README.md` for your `tanzaniasafari` project, assuming it’s a **Node.js REST API for a social app**.

---

```markdown
# 🧭 Tanzania Safari - Social App API

Welcome to the backend API for the Tanzania Safari Social App — a Node.js + Express REST API designed to handle core social networking features like user registration, authentication, post creation, likes, follows, and more.

---

## 🚀 Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/pravinpgr9/tanzaniasafari.git
   cd tanzaniasafari
   ```

2. **Install dependencies:**
   ```bash
   yarn install
   # or
   npm install
   ```

3. **Create an `.env` file** with your MongoDB URI and port config (example below):
   ```
   MONGO_URL=mongodb://localhost:27017/socialapp
   PORT=8808
   ```

4. **Start the server:**
   ```bash
   yarn start
   # or
   npm start
   ```

---

## 📌 API Endpoints

---

### 📫 **Posts API**

#### 1. Delete Post
- **Method:** `DELETE`
- **URL:** `/api/posts/:postId`
- **Body:**
  ```json
  {
    "userId": "USER_ID"
  }
  ```

#### 2. Like / Unlike Post
- **Method:** `PUT`
- **URL:** `/api/posts/:postId/like`
- **Body:**
  ```json
  {
    "userId": "USER_ID"
  }
  ```

#### 3. Create Post
- **Method:** `POST`
- **URL:** `/api/post`
- **Body:**
  ```json
  {
    "userId": "USER_ID",
    "desc": "Description of the post",
    "img": "https://example.com/image.jpg",
    "likes": []
  }
  ```

#### 4. Get User Timeline
- **Method:** `GET`
- **URL:** `/api/posts/timeline/:userId`

#### 5. Get All Posts
- **Method:** `GET`
- **URL:** `/api/posts`

#### 6. Get Single Post
- **Method:** `GET`
- **URL:** `/api/posts/:postId`

---

### 👤 **User API**

#### 1. Register User
- **Method:** `POST`
- **URL:** `/api/auth/register`
- **Body:**
  ```json
  {
    "username": "pravinpgr1998",
    "email": "pravinpgr1998@gmail.com",
    "password": "demotest"
  }
  ```

#### 2. Login
- **Method:** `POST`
- **URL:** `/api/auth/login`
- **Body:**
  ```json
  {
    "username": "pravinpgr12",
    "password": "demotest"
  }
  ```

#### 3. Update User
- **Method:** `PUT`
- **URL:** `/api/user/:userId`
- **Body:**
  ```json
  {
    "userId": "USER_ID",
    "username": "newusername"
  }
  ```

#### 4. Delete User
- **Method:** `DELETE`
- **URL:** `/api/user/:userId`
- **Body:**
  ```json
  {
    "userId": "USER_ID"
  }
  ```

#### 5. Follow a User
- **Method:** `PUT`
- **URL:** `/api/user/:userId/follow`
- **Body:**
  ```json
  {
    "userId": "FOLLOWER_ID"
  }
  ```

#### 6. Unfollow a User
- **Method:** `PUT`
- **URL:** `/api/user/:userId/unfollow`
- **Body:**
  ```json
  {
    "userId": "FOLLOWER_ID"
  }
  ```

#### 7. Get User Details
- **Method:** `GET`
- **URL:** `/api/user/:userId`

---

## 🧾 Sample Environment File `.env`

```env
MONGO_URL=mongodb://localhost:27017/socialapp
PORT=8808
```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙌 Author

Made with ❤️ by [Pravin Pagare](https://github.com/pravinpgr9)
```

---

Let me know if you'd like to add Postman collection links, Swagger docs, or frontend repo references too!