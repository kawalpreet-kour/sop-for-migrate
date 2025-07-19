# SOP: Step-by-Step Installation Guide for Migrate

A comprehensive step-by-step guide for installing `migrate` on Debian/Ubuntu-based Linux systems.

---

| Authors           | Created on     | Version | Last updated by | Last edited on |
|-------------------|---------------|---------|-----------------|---------------|
| Kawalpreet Kour   | 19 July 2025  | v1      | -               | -             |

---
## Table of Contents

1. [Introduction](#introduction)  
2. [Scope](#scope)  
3. [Prerequisites](#prerequisites)  
4. [Procedure](#procedure)  
   - [Step 1: Update System Packages](#step-1-update-system-packages)  
   - [Step 2: Install curl if not already installed](#step-2-install-curl-if-not-already-installed)  
   - [Step 3: Add the Golang Migrate Repository](#step-3-add-the-golang-migrate-repository)  
   - [Step 4: Update the Package List](#step-4-update-the-package-list)  
   - [Step 5: Install migrate CLI](#step-5-install-migrate-cli)  
   - [Step 6: Verify the Installation](#step-6-verify-the-installation)  
5. [Notes](#notes)  
6. [Conclusion](#conclusion)  
7. [Contact](#contact)  
8. [References](#references)  

---

## Introduction

Golang Migrate is a powerful command-line tool used to manage and apply database migrations. This tool supports multiple databases including PostgreSQL, MySQL, SQLite, and more. This SOP will guide you through the installation of the `migrate` CLI on Ubuntu/Debian systems.

---

## Scope

This SOP covers **only the installation** of the `migrate` tool. 

---

## Prerequisites

- Ubuntu 20.04+ or Debian-based system  
- Terminal access with `sudo` privileges  
- Internet connection  
- Basic understanding of Linux commands

---

## Procedure

### Step 1: Update System Packages

```bash
sudo apt-get update 
```
<img width="1304" height="495" alt="Screenshot from 2025-07-20 00-11-17" src="https://github.com/user-attachments/assets/6f0cf1a2-afae-41d0-bc46-76ae9b55cc62" />

This ensures your system is using the latest package lists.

## Step 2: Let us setup the repository to install the migrate package.
```bash
 curl -s https://packagecloud.io/install/repositories/golang-migrate/migrate/script.deb.sh | sudo bash 
```


### Step 3: Update System Packages Again

```bash
sudo apt-get update 
```
<img width="1304" height="495" alt="Screenshot from 2025-07-20 00-11-17" src="https://github.com/user-attachments/assets/6f0cf1a2-afae-41d0-bc46-76ae9b55cc62" />

### Step 4: install migrate

```bash
sudo apt-get install migrate
```
<img width="1080" height="393" alt="Screenshot from 2025-07-20 00-13-11" src="https://github.com/user-attachments/assets/97037ba7-9e0f-458a-b7cf-935bc7fbfd2d" />

### Step 5: Verify Installation

```bash
migrate -version
```
<img width="672" height="86" alt="Screenshot from 2025-07-20 00-13-44" src="https://github.com/user-attachments/assets/66c4d7b0-81d1-4249-9810-132fc2d357b9" />
 
-This Confirms that migrate was installed correctly.

---

## Contact Information

| Name             | Email                                         |
|------------------|-----------------------------------------------|
| Kawalpreet Kour  | Kawalpreet.kour.snaatak@mygurukulam.co        |

---
