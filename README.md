# SOP: Installation Guide for Migrate

This SOP covers only the installation of the `migrate`tool on Debian/Ubuntu systems.


---
## Author Information
| Last Updated On | Version | Author           | Level           | Reviewer               |
|-----------------|---------|------------------|-----------------|------------------------|
| 18-07-2025      | V1.0    | Kawalpreet Kour  | Internal Review | Pritam                 |
| 25-07-2025      | V1.1    | Kawalpreet Kour  | L0              | Shreya/Sharvani        |
|                 |         | Kawalpreet Kour  | L1              | Abhishek V             |
|                 |         | Kawalpreet Kour  | L2              | Abhishek Dubey/Rishabh sharma |

---

## Introduction

Golang Migrate is a powerful command-line tool used to manage and apply database migrations. It supports multiple databases including PostgreSQL, MySQL, SQLite, and others.

---

## Table of Contents

- [Purpose](#purpose)  
- [Pre-requisites](#pre-requisites)  
- [Procedure](#procedure)  
  - [Update System Packages](#update-system-packages)  
  - [Add the Golang Migrate Repository](#add-the-golang-migrate-repository)  
  - [Update System Packages Again](#update-system-packages-again)  
  - [Install migrate CLI](#install-migrate-cli)  
  - [Verify the Installation](#verify-the-installation)  
- [Notes](#notes)  
- [Conclusion](#conclusion)  
- [Contact Information](#contact-information)  
- [References](#references)
---



## Purpose

A comprehensive, step-by-step guide for installing the `migrate` command-line tool on Debian/Ubuntu-based Linux systems.

---

## Pre-requisites

| Component             | Description                                                     |
|-----------------------|-----------------------------------------------------------------|
| Linux System          | Ubuntu 20.04+ or any Debian-based system is required            |
| Sudo Privileges       | You must have terminal access with `sudo` permissions           |
| Command-line Basics   | Basic familiarity with Linux commands and terminal navigation   |

---

## Procedure

### Update System Packages

Open your terminal and run the following command to refresh your package lists:

```bash
sudo apt-get update
```
<img width="1304" height="495" alt="Screenshot from 2025-07-20 00-11-17" src="https://github.com/user-attachments/assets/6f0cf1a2-afae-41d0-bc46-76ae9b55cc62" />

---

### Add the Golang Migrate Repository

Set up the official repository for Golang Migrate:

```bash
curl -s https://packagecloud.io/install/repositories/golang-migrate/migrate/script.deb.sh | sudo bash
```

---

### Update System Packages Again

After adding the repository, update the package list again:

```bash
sudo apt-get update
```
<img width="1304" height="495" alt="Screenshot from 2025-07-20 00-11-17" src="https://github.com/user-attachments/assets/6f0cf1a2-afae-41d0-bc46-76ae9b55cc62" />

---

### Install migrate CLI

Install the `migrate` command-line tool:

```bash
sudo apt-get install migrate
```
<img width="1080" height="393" alt="Screenshot from 2025-07-20 00-13-11" src="https://github.com/user-attachments/assets/97037ba7-9e0f-458a-b7cf-935bc7fbfd2d" />

---

### Verify the Installation

Check that `migrate` is installed and working:

```bash
migrate -version
```
<img width="672" height="86" alt="Screenshot from 2025-07-20 00-13-44" src="https://github.com/user-attachments/assets/66c4d7b0-81d1-4249-9810-132fc2d357b9" />

If the version number is displayed, the installation was successful.

---

## Notes

| Point No. | Description                                                                 |
|-----------|-----------------------------------------------------------------------------|
| 1         | If you encounter issues, ensure your system time and date are correct and that you have a working internet connection. |
| 2         | The repository script automatically configures the correct source for your OS version. |

---

## Conclusion

Following these steps, you should have successfully installed the `migrate` CLI on your Debian/Ubuntu system. You can now use it to manage your database migrations efficiently.

---
## Contact Information

| Name             | Email                                         |
|------------------|-----------------------------------------------|
| Kawalpreet Kour  | Kawalpreet.kour.snaatak@mygurukulam.co        |

---
## References

| Title                                               | Link                                                                                  |
|-----------------------------------------------------|---------------------------------------------------------------------------------------|
| Golang Migrate Documentation                        | [Visit GitHub](https://github.com/golang-migrate/migrate)                            |
| GFG: Install Golang Migrate on Ubuntu               | [Read on GeeksforGeeks](https://www.geeksforgeeks.org/installation-guide/how-to-install-golang-migrate-on-ubuntu/) |



