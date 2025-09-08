# 🍜 Flavors of Malaysia - A WordPress Food Promotion Website

This project is a one-page website developed using WordPress and Elementor to promote the diverse and rich culinary heritage of Malaysia. The site serves as a comprehensive guide for food enthusiasts, tourists, and locals looking for authentic Malaysian food recommendations and recipes.
<br><br>

### ✨ Features
- **One-Page Design**: A seamless, user-friendly, single-page layout with smooth-scrolling navigation.
- **Dynamic Hero Section**: A high-impact hero section with a high-quality background image and a clear call-to-action to engage visitors immediately.
- **Top Dishes Showcase**: Features five must-try Malaysian dishes, each with a high-quality image and a detailed description of its ingredients, flavors, and cultural significance.
- **Interactive Recipe Guides**: Provides three detailed, step-by-step recipes for popular Malaysian dishes, complete with an image carousel for visual instructions.
- **Downloadable Recipe PDFs**: Each recipe includes a "Download as PDF" button, linking to a custom-formatted PDF for offline use.
- **Blog Integration**: An optional blog section with excerpts from relevant articles and "Read More" links to external pages.
- **Interactive Contact Section**: Includes a functional contact form, social media links, and an embedded Google Map for location reference.
<br>

### 🛠️ Technical Overview
- **Platform**: WordPress
- **Page Builder**: Elementor
- **Hosting**: Locally hosted development environment (XAMPP)
<br>

### 🎥 Functional Walkthrough
A complete video demonstration of the website's features, navigation and functionality is available at [here](https://youtu.be/PU_guG74S0U).

<p align="center">
    <a href="https://youtu.be/PU_guG74S0U">
        <img src="https://github.com/user-attachments/assets/dab02c70-d44b-48c1-a13c-381c9d43f416" alt="Watch the Functional Walkthrough Video" width="500"/>
    </a>
</p>
<br>

### 📁 File Structure
- **`myblog.zip` (108 MB)**: A compressed archive with all WordPress files. Due to its size, this file is hosted externally. [➡️ Download Website Files Here](https://drive.google.com/file/d/1fqK9MaGHuMH7PN-NIqPw0iNFVoRMRNN5/view?usp=sharing)
- **`myblogdb.sql`**: The SQL database backup file containing all the website's content, settings, and user data.
- **`Report.pdf`**: The full academic report detailing the design, implementation, and features of each website section.
<br>

### 🚀 Getting Started: Setting Up the Website Locally

Since this website was developed on a local server, follow these steps to set it up in own local environment.

> **Prerequisites:**
> A local server environment is needed to be installed on computer. **[XAMPP](https://www.apachefriends.org/index.html)** is a great free option that includes Apache (web server) and MySQL (database).

**Step-by-Step Guide:**

1.  **🖥️ Start Local Server**
    -   Open the XAMPP Control Panel.
    -   Start the **Apache** and **MySQL** services.

2.  **📂 Download and Place the Website Files**
    -   Download the **`myblog.zip`** (108 MB) file from the link provided in the `File Structure` section above.
    -   Unzip the downloaded file. This will create a folder named `myblog`.
    -   Move the entire `myblog` folder into the `htdocs` directory inside the XAMPP installation folder (e.g., `C:/xampp/htdocs/`).

3.  **🗃️ Create and Import the Database**
    -   Open web browser and go to `http://localhost/phpmyadmin`.
    -   Click on **New** to create a new database. Name it **`myblogdb`** and click "Create".
    -   Select the `myblogdb` database that just created from the left-hand sidebar.
    -   Click on the **Import** tab at the top.
    -   Click "Choose File" and select the **`myblogdb.sql`** file from this repository.
    -   Scroll down and click **Go** to start the import. Wait for it to complete.

4.  **🔗 Connect WordPress to the Database**
    -   Navigate to the website files folder: `C:/xampp/htdocs/myblog`.
    -   Find the file named **`wp-config.php`** and open it in a text editor.
    -   Update the following lines to match the local database settings (for a default XAMPP setup, the user is `root` with no password):
        ```php
        /** The name of the database for WordPress */
        define( 'DB_NAME', 'myblogdb' );

        /** Database username */
        define( 'DB_USER', 'root' );

        /** Database password */
        define( 'DB_PASSWORD', '' );
        ```
    -   Save and close the `wp-config.php` file.

5.  **🎉 View the Website!**
    -   Open web browser and navigate to **`http://localhost/myblog`**.
    -   The "Flavors of Malaysia" website should now be running locally!
<br>

### 🔍 Website Sections Overview
1.  **Header & Hero Section**:
    -   **Header**: Features the website title (Flavors of Malaysia) and a clean navigation menu with anchor links (Home, About, Top Dishes, Recipes, Contact).
    -   **Hero**: A full-width image of iconic Malaysian dishes, an introductory tagline, and a primary "Explore Top Dishes" call-to-action button.

2.  **About Section**:
    -   Provides context with a mission statement, a brief history of Malaysian cuisine, and a summary of its key cultural influences (Malay, Chinese, Indian, etc.).

3.  **Top Dishes & Recipes**:
    -   **Top Dishes**: A visually rich section showcasing 5 iconic dishes with detailed descriptions.
    -   **Recipes**: Step-by-step guides for 3 popular recipes, complete with image carousels and downloadable PDFs.

4.  **Blog, Contact & Footer**:
    -   **Blog**: Excerpts of food-related articles to provide additional content.
    -   **Contact**: A section with a contact form, social media icons, and an embedded map.
    -   **Footer**: Contains a secondary navigation menu, social media icons, and copyright information.
<br>
