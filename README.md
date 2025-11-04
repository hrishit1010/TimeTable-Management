# TimeTable-Management


This project is a standalone, offline desktop application designed to generate and manage timetables for universities and colleges. It provides a robust solution for creating complex, logical schedules while handling various constraints.

## 📖 About This Project

The purpose of this application is to provide an efficient tool for universities and colleges to generate advanced, logical timetables. It is built to run offline as a desktop application.

## ✨ Key Features

* **Offline First:** Operates as a standalone desktop application using Electron.
* **Complex Constraint Handling:** Manages complex scheduling rules, including:
    * Parallel sessions
    * Conservative (back-to-back) sessions
    * Session overlap prevention
* **Availability Management:** Accounts for "not available" times for lecturers, rooms, and student groups.

## 🛠️ Tech Stack

* **Framework:** [Electron](https://www.electronjs.org/)
* **Database ORM:** [Sequelize](https://sequelize.org/) (with SQLite)
* **Frontend & UI:**
    * [Bootstrap](https://getbootstrap.com/)
    * [jQuery](https://jquery.com/)
    * [jQuery DataTables](https://datatables.net/)
    * [jquery-confirm.js](https://craftpip.github.io/jquery-confirm/)

## 🚀 Getting Started

Follow these instructions to get the project up and running on your local machine for development and testing.

### Prerequisites

Before you begin, ensure you have the following installed on your system:
* [Node.js](https://nodejs.org/en) (which includes npm)

### Installation & Setup

1.  **Install dependencies:**
    From the project's root folder, run `npm install` to install all necessary packages.
    ```bash
    npm install
    ```

2.  **Initialize the database:**
    a.  Navigate to the `src` folder:
        ```bash
        cd src
        ```
    b.  Run the database migration to create the database schema:
        ```bash
        npx sequelize-cli db:migrate
        ```
    c.  This will create a `schedule.sqlite3` file inside the `src` folder. **Move this file** to the `database/` folder located in the project's root directory.
    d.  Return to the root folder:
        ```bash
        cd ..
        ```

3.  **Run the application:**
    From the root folder, run `npm start` to launch the Electron application.
    ```bash
    npm start
    ```

## 📸 Screenshots

<img width="1920" height="1040" alt="image" src="https://github.com/user-attachments/assets/4c57d932-9306-4535-bb74-6adffab81799" />
<img width="1920" height="1040" alt="image" src="https://github.com/user-attachments/assets/949424c2-2bab-4a7a-b4bc-41f5b8dd779f" />
<img width="1920" height="1040" alt="image" src="https://github.com/user-attachments/assets/1a558d8f-d270-48f1-a915-0bfc759c96c9" />
<img width="1920" height="1040" alt="image" src="https://github.com/user-attachments/assets/189a76aa-4e29-4142-909d-0218339d18d5" />

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request
