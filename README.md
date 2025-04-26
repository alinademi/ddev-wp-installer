# 🧰 DDEV WordPress Installer Add-on

[![DDEV Add-on](https://img.shields.io/badge/DDEV-Add--on-blue?logo=ddev)](https://ddev.com)
[![GitHub release](https://img.shields.io/github/v/release/alinademi/ddev-wp-installer)](https://github.com/alinademi/ddev-wp-installer/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This DDEV add-on provides a friendly way to install WordPress in either:

- 🔥 **YOLO mode** — using your Git info and a randomly generated admin password
- 🛠 **Details mode** — interactively set title, username, password, and email

## 🚀 Quick Start

```bash
ddev get alinademi/ddev-wp-installer
ddev wp-install
```

## 🔧 Features

- Uses your Git `user.name` and `user.email` for defaults (YOLO mode)
- Generates secure passwords automatically
- Works on fresh WordPress projects in DDEV

## 📦 Installation Options

### Option 1: Via GitHub

```bash
ddev get alinademi/ddev-wp-installer
```

### Option 2: Local Development

Clone the repo and link it into your project:

```bash
git clone https://github.com/alinademi/ddev-wp-installer.git
cd my-ddev-project
ddev get ../ddev-wp-installer
```

## 🧪 Usage

```bash
ddev wp-install
```

You will be prompted to choose:

```txt
1) YOLO (auto-install with Git info)
2) Details (prompt for each field)
3) Exit
```

### YOLO Mode Output Example

```txt
✅ WordPress installed in YOLO mode!
🔐 Admin credentials:
   Username: admin
   Password: Rnd0mP@ssW0rd!

📢 Please copy and store this password securely — you won’t see it again!
```

### 📚 Test Content Import

After installation, you can choose to import WordPress Theme Unit Test content. This includes:

- Sample posts and pages
- Comments and nested comments
- Categories and tags
- Images and media
- Custom menus
- Theme testing data

The importer will:

- Download official WordPress Theme Unit Test data
- Install and activate WordPress Importer plugin
- Import all test content

To import test content separately:

```bash
ddev wp-test-content
```

## 🙋‍♀️ Contributing

PRs and issues welcome! This is a community-friendly DDEV add-on.  
Make sure to test with the latest version of DDEV:

```bash
ddev --version
```

## 📝 License

MIT — use freely, modify freely, contribute freely.
