# Task Manager CRUD App

A simple **Task Manager** application built using **Ruby on Rails** with full CRUD (Create, Read, Update, Delete) functionality.

## Features
- Create, Read, Update, and Delete (CRUD) tasks
- Mark tasks as completed or pending
- Inline CSS for styling
- Deployed on **Render / Fly.io**

---

## Installation
### Prerequisites
Ensure you have the following installed:
- Ruby (>= 3.0.0)
- Rails (>= 7.0)
- PostgreSQL (or SQLite for local development)
- Git

### Steps to Run Locally
1. **Clone the repository**
   ```sh
   git clone <your-repo-url>
   cd task-manager
   ```

2. **Install dependencies**
   ```sh
   bundle install
   ```

3. **Set up the database**
   ```sh
   rails db:create db:migrate db:seed
   ```

4. **Start the Rails server**
   ```sh
   rails server
   ```
   The app will be available at **http://localhost:3000/tasks**

---

## Usage
- Visit **`/tasks`** to view all tasks
- Click **New Task** to create a task
- Click **Edit** to update a task
- Click **Delete** to remove a task

---

## Deployment
### Deploy to **Render** (Recommended)
1. Push your code to **GitHub**:
   ```sh
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```
2. Sign up on **[Render](https://render.com/)** and create a **Web Service**
3. Connect your GitHub repository and set:
   - **Build Command:** `bundle install && rails db:migrate`
   - **Start Command:** `rails server -b 0.0.0.0`
4. Deploy and get a live URL!

### Deploy to **Fly.io**
1. Install Fly CLI:
   ```sh
   curl -fsSL https://get.fly.io/install.sh | sh
   ```
2. Authenticate & Create App:
   ```sh
   flyctl auth signup
   flyctl launch
   ```
3. Deploy:
   ```sh
   flyctl deploy
   ```

---

## Contributing
1. Fork the repository
2. Create a feature branch (`git checkout -b new-feature`)
3. Commit changes (`git commit -m "Add new feature"`)
4. Push to GitHub (`git push origin new-feature`)
5. Open a **Pull Request**

---

## License
This project is open-source and available under the **MIT License**.

---

## Contact
For questions or suggestions, feel free to open an **issue** or reach out via email.

🚀 Happy Coding!
