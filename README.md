# SOP: Step-by-Step Installation Guide for Migrate

A comprehensive, step-by-step guide for installing the `migrate` command-line tool on Debian/Ubuntu-based Linux systems.

---

| Authors           | Created on    | Version | Last updated by | Last edited on |
|-------------------|--------------|---------|-----------------|---------------|
| Kawalpreet Kour   | 19 July 2025 | v1      | -               | -             |

---

## Table of Contents

1. [Introduction](#introduction)  
2. [Scope](#scope)  
3. [Prerequisites](#prerequisites)  
4. [Procedure](#procedure)  
    - [Step 1: Update System Packages](#step-1-update-system-packages)  
    - [Step 2: Add the Golang Migrate Repository](#step-2-add-the-golang-migrate-repository)  
    - [Step 3: Update System Packages Again](#step-3-update-system-packages-again)  
    - [Step 4: Install migrate CLI](#step-4-install-migrate-cli)  
    - [Step 5: Verify the Installation](#step-5-verify-the-installation)  
5. [Notes](#notes)  
6. [Conclusion](#conclusion)  
7. [Contact](#contact-information)  
8. [References](#references)  

---

## Introduction

[Golang Migrate](https://github.com/golang-migrate/migrate) is a powerful command-line tool used to manage and apply database migrations. It supports multiple databases including PostgreSQL, MySQL, SQLite, and others. This SOP guides you through a reliable process for installing the `migrate` CLI on Ubuntu/Debian-based systems.

---

## Scope

This SOP covers **only the installation** of the `migrate` CLI tool on Debian/Ubuntu systems.

---

## Prerequisites

- Ubuntu 20.04+ or Debian-based system  
- Terminal access with `sudo` privileges  
- Internet connection  
- Basic familiarity with Linux command line

---

## Procedure

### Step 1: Update System Packages

Open your terminal and run the following command to refresh your package lists:

```bash
sudo apt-get update
```
<img width="1304" height="495" alt="Screenshot from 2025-07-20 00-11-17" src="https://github.com/user-attachments/assets/6f0cf1a2-afae-41d0-bc46-76ae9b55cc62" />

---

### Step 2: Add the Golang Migrate Repository

Set up the official repository for Golang Migrate:

```bash
curl -s https://packagecloud.io/install/repositories/golang-migrate/migrate/script.deb.sh | sudo bash
```

---

### Step 3: Update System Packages Again

After adding the repository, update the package list again:

```bash
sudo apt-get update
```
<img width="1304" height="495" alt="Screenshot from 2025-07-20 00-11-17" src="https://github.com/user-attachments/assets/6f0cf1a2-afae-41d0-bc46-76ae9b55cc62" />

---

### Step 4: Install migrate CLI

Install the `migrate` command-line tool:

```bash
sudo apt-get install migrate
```
<img width="1080" height="393" alt="Screenshot from 2025-07-20 00-13-11" src="https://github.com/user-attachments/assets/97037ba7-9e0f-458a-b7cf-935bc7fbfd2d" />

---

### Step 5: Verify the Installation

Check that `migrate` is installed and working:

```bash
migrate -version
```
<img width="672" height="86" alt="Screenshot from 2025-07-20 00-13-44" src="https://github.com/user-attachments/assets/66c4d7b0-81d1-4249-9810-132fc2d357b9" />

If the version number is displayed, the installation was successful.

---

## Notes

- If you encounter issues, ensure your system time and date are correct and that you have a working internet connection.
- The repository script automatically configures the correct source for your OS version.

---

## Conclusion

Following these steps, you should have successfully installed the `migrate` CLI on your Debian/Ubuntu system. You can now use it to manage your database migrations efficiently.

---

## References

- [Golang Migrate Documentation](https://github.com/golang-migrate/migrate)
- [GeeksforGeeks: How to Install Golang Migrate on Ubuntu](https://www.geeksforgeeks.org/installation-guide/how-to-install-golang-migrate-on-ubuntu/)

---

## Contact Information

| Name             | Email                                         |
|------------------|-----------------------------------------------|
| Kawalpreet Kour  | Kawalpreet.kour.snaatak@mygurukulam.co        |

---

