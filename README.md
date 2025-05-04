# OS Project

Welcome to the **OS Project**, a React-based application built using **Vite**. This project showcases modern web development practices and offers a robust setup for building, deploying, and maintaining React applications.

---

## 📑 Table of Contents

* [Introduction](#introduction)
* [Features](#features)
* [Technologies Used](#technologies-used)
* [Setup and Installation](#setup-and-installation)
* [Usage](#usage)
* [Scripts](#scripts)
* [Test and Set (Hardware Synchronization)](#test-and-set-hardware-synchronization)
* [Swapping (Hardware Synchronization)](#swapping-hardware-synchronization)
* [Contributing](#contributing)

---

## 🔰 Introduction

This project is designed to provide a **minimal and efficient setup** to develop and deploy React applications.
It leverages **Vite** for fast builds and a development server, along with **ESLint** for maintaining code quality.

---

## ✨ Features

* **React Integration** → Built with React for modular and component-based development.
* **Fast Development** → Uses Vite for lightning-fast build times and Hot Module Replacement (HMR).
* **Code Quality** → Includes ESLint configuration to enforce clean, consistent coding standards.
* **Deployment Ready** → Configured for seamless deployment to GitHub Pages.
* **Routing** → Utilizes `react-router-dom` for smooth client-side routing.

---

## 🛠️ Technologies Used

* **React** → JavaScript library for building user interfaces.
* **Vite** → Modern build tool and development server.
* **React Icons** → Scalable vector icons.
* **React Router** → Declarative routing for React apps.
* **ESLint** → Tool for identifying and fixing code quality issues.

---

## ⚙️ Setup and Installation

Clone the repository:

```bash
git clone https://github.com/phitesh1912/osproject.git
cd osproject
```

Install dependencies:

```bash
npm install
```

---

## 🚀 Usage

Start the development server:

```bash
npm run dev
```

Build the application for production:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

---

## 📜 Scripts

| Script            | Description                             |
| ----------------- | --------------------------------------- |
| `npm run dev`     | Starts the development server with HMR. |
| `npm run build`   | Builds the project for production.      |
| `npm run lint`    | Runs ESLint for code linting.           |
| `npm run preview` | Serves the built project locally.       |
| `npm run deploy`  | Deploys the project to GitHub Pages.    |

---

## 🔒 Test and Set (Hardware Synchronization)

The **Test and Set** instruction is a fundamental hardware-based synchronization mechanism used to achieve **mutual exclusion** in multiprocessor systems.
It’s implemented directly in hardware to ensure **atomicity** and prevent race conditions.

### How It Works:

* **Test Phase** → The current value of a lock variable is read (tested).
* **Set Phase** → If the value indicates the lock is free, it’s set to a locked state in the same atomic operation.

This atomic operation ensures that no two processes can simultaneously change the lock's state, even in a multiprocessor environment.

### Applications:

* Implementing critical sections in operating systems.
* Ensuring only one process accesses shared resources at a time.

### Advantages:

✅ Simple and efficient for hardware-level synchronization.
✅ Effectively prevents race conditions.

### Disadvantages:

⚠ Can lead to **busy-waiting**, where a process continuously checks the lock, consuming CPU resources.

---

## 🔄 Swapping (Hardware Synchronization)

**Swapping** in hardware synchronization refers to the atomic exchange of values between two memory locations, another primitive used for **mutual exclusion** and managing concurrent access.

### How It Works:

* Two values (e.g., a lock variable and a flag) are swapped atomically by the hardware.
* If the lock is free, the process swaps its flag with the lock, effectively acquiring the lock.

### Applications:

* Implementing **spinlocks** or other synchronization primitives in operating systems.
* Ensuring mutual exclusion in multiprocessor environments.

### Advantages:

✅ Eliminates the need for complex software-based synchronization mechanisms.
✅ Guarantees atomicity through hardware.

### Disadvantages:

⚠ Similar to **Test and Set**, it can result in busy-waiting.
⚠ Requires hardware support for atomic swap operations.

---

## 🤝 Contributing

If you’d like to contribute to this project:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.
