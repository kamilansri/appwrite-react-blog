# BlogWrite ✍️

A modern, fast, and fully functional blog editor application built with React, Vite, and Appwrite. 

This project allows users to create accounts, write rich-text blog posts, upload cover images, and manage their content securely. It leverages Appwrite as a complete Backend-as-a-Service (BaaS) to handle authentication, database operations, and file storage.

## ✨ Features

* **User Authentication:** Secure login, signup, and logout functionality.
* **Rich Text Editing:** Integrated editor to write and format blog posts seamlessly.
* **CRUD Operations:** Create, Read, Update, and Delete your own blog posts.
* **Image Storage:** Upload and manage cover images for articles.
* **Responsive Design:** Optimized for both desktop and mobile viewing.
* **Protected Routes:** Ensure only authenticated users can access the editor and dashboard.

## 🛠️ Tech Stack

* **Frontend:** React (Bootstrapped with Vite)
* **Routing:** React Router DOM
* **State Management:** Redux Toolkit / React Context (Update based on your choice)
* **Backend / BaaS:** Appwrite (Auth, Databases, Storage)
* **Styling:** Tailwind CSS (Update if using standard CSS/SCSS)
* **Rich Text Editor:** TinyMCE / React Quill (Update based on your choice)

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

* Node.js installed on your machine.
* An [Appwrite](https://appwrite.io/) account and a project set up.

### Installation

1.  **Clone the repository:**
    ```
    git clone https://github.com/kamilansri/appwrite-react-blog.git
    
    cd your-repo-name
  

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Set up Environment Variables:**
    Create a `.env` file in the root of your project and add your Appwrite configuration details. *Note: Do not commit this file to GitHub.*

    ```env
    VITE_APPWRITE_URL="your-appwrite-endpoint"
    VITE_APPWRITE_PROJECT_ID="your-project-id"
    VITE_APPWRITE_DATABASE_ID="your-database-id"
    VITE_APPWRITE_COLLECTION_ID="your-collection-id"
    VITE_APPWRITE_BUCKET_ID="your-bucket-id"
    ```

4.  **Start the development server:**
    ```bash
    npm run dev
    ```

## 🗄️ Appwrite Setup Guide

To make this project work, you need to configure your Appwrite backend:

1.  **Create a Project** in your Appwrite console.
2.  **Create a Database** and note down the Database ID.
3.  **Create a Collection** (e.g., "Articles") within that database and note the Collection ID.
4.  **Set up Attributes** for your collection (e.g., `title` (string), `content` (string), `featuredImage` (string), `status` (string), `userId` (string)).
5.  **Create a Storage Bucket** for uploading images and note the Bucket ID.
6.  **Update Permissions:** Ensure you set the correct read/write permissions for your collection and bucket so authenticated users can interact with them.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/your-username/your-repo-name/issues).

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
