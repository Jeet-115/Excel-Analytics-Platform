# Contributing to Sheet Sense

Thank you for your interest in contributing to **Sheet Sense**! We welcome contributions from developers, designers, testers, and data enthusiasts. By contributing, you help improve the platform for everyone.

---

## 📝 How to Contribute

### 1. Reporting Issues

If you find a bug or have a suggestion for improvement:

1. Check the [Issues](https://github.com/<your-username>/sheetsense/issues) page to see if it already exists.
2. If not, create a new issue with:

   * Clear description of the problem
   * Steps to reproduce (if applicable)
   * Screenshots (optional)
   * Expected behavior vs actual behavior

---

### 2. Submitting Pull Requests (PRs)

#### Step 1: Fork the Repository

* Click on **Fork** in the top-right corner to create your own copy.

#### Step 2: Clone Your Fork

```bash
git clone https://github.com/<your-username>/sheetsense.git
cd sheetsense
```

#### Step 3: Create a Branch

* Always create a new branch for your work:

```bash
git checkout -b feature/your-feature-name
```

#### Step 4: Make Your Changes

* Follow **coding conventions** and **folder structure**.
* Frontend: React + Redux + Tailwind + Chart.js/Recharts/Three.js
* Backend: Node.js + Express + MongoDB + Mongoose + JWT + AI integration

#### Step 5: Commit Your Changes

```bash
git add .
git commit -m "Add brief description of your changes"
```

#### Step 6: Push and Create PR

```bash
git push origin feature/your-feature-name
```

* Open a **Pull Request** from your branch to the `main` branch.
* Provide a detailed description of your changes and link related issues if any.

---

### 3. Code Style and Guidelines

* **Frontend:** Follow the existing React + Tailwind + Chart component structure.
* **Backend:** Follow Express + Mongoose structure with controllers, routes, and models.
* Use descriptive variable and function names.
* Write comments for complex logic, AI interactions, or Excel data handling.
* Ensure no sensitive data (like `.env` variables or API keys) is committed.

---

### 4. Testing

* Test your code before submitting PRs.
* Manual testing is sufficient for frontend/backend functionality.
* Check CRUD operations for Excel uploads, AI insights, chart generation, and admin/user workflows.

---

### 5. Communication

* Open issues or pull requests for questions or discussions.
* Mention contributors using `@username` in PR comments if needed.
* Be respectful and constructive in all interactions.

---

### 6. Additional Contributions

* UI/UX improvements
* Documentation updates
* Adding new chart types or AI insights
* Performance optimizations
* Multilingual support improvements

---

## 🙌 Need Help?

If you’re unsure about anything:

* Open an issue with the label `question`
* Or reach out via the project maintainers’ contact in the Code of Conduct.

Thanks for contributing to **Sheet Sense**! 💜
