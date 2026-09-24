# Cloud Deployment – Employee Security Checker

## About This Project

This project shows how I deployed and tested my Java Employee Security Checker application on an **AWS EC2 Linux server**.

The application checks an employee's basic security training and gives the employee a security score and risk level.

This project was created to demonstrate my practical Cloud Computing skills by taking a Java application from GitHub and running it on an AWS cloud server.

## Cloud Platform

**Amazon Web Services (AWS)**

Service used:

* Amazon EC2
* Amazon Linux
* SSH

## What I Did

### 1. Created an AWS EC2 Instance

I created an EC2 virtual server on AWS.

The instance was configured with:

* Instance name: Employee-Security-Checker
* Instance type: t3.micro
* Operating system: Amazon Linux
* Region: Asia Pacific (Mumbai)
* SSH access using an EC2 key pair

### 2. Connected to the EC2 Server

I connected to the Linux server from my Windows computer using SSH.

This allowed me to work directly on the AWS server through the terminal.

### 3. Installed the Required Tools

I installed the software needed to run my Java project:

* Git
* Java 17
* Maven

I used Git to download my project from GitHub.

### 4. Cloned My Project

I cloned my Employee Security Checker project from GitHub onto the EC2 server.

The project was downloaded using:

```bash
git clone https://github.com/NoxoloBojana/employee-security-checker.git
```

### 5. Ran the Tests

After downloading the project, I used Maven to run the automated tests:

```bash
mvn test
```

The tests completed successfully.

### 6. Compiled the Application

I compiled the Java application on the AWS server using:

```bash
mvn compile
```

The project compiled successfully.

### 7. Ran the Application on AWS

I then ran the Employee Security Checker directly on the EC2 server using Java.

The application accepted employee information and produced a security score and risk level.

Example:

```text
Employee: Noxolo
Security Score: 2/3
Risk Level: MEDIUM RISK
```

## What I Learned

Through this project I learned how to:

* Create an AWS EC2 instance
* Connect to a cloud Linux server using SSH
* Work with a remote server
* Install Java, Git and Maven on a cloud server
* Clone a GitHub project onto an EC2 instance
* Run automated tests on a cloud server
* Compile and run a Java application on AWS
* Understand how a cloud server can be used to host and run software

## Project Structure

The original Employee Security Checker project contains:

```text
Employee Security Checker
│
├── Employee
├── SecurityChecker
├── SecurityReport
├── EmployeeSecurityChecker
└── Tests
```

The application uses employee security information to calculate a score out of 3.

### Risk Levels

| Score | Risk Level  |
| ----- | ----------- |
| 3/3   | LOW RISK    |
| 2/3   | MEDIUM RISK |
| 0–1/3 | HIGH RISK   |

## Evidence

This repository documents the AWS deployment work I completed.

The original application source code is available in my Employee Security Checker repository:

https://github.com/NoxoloBojana/employee-security-checker

## Proof of Work

The following Google Drive folder contains screenshots showing my AWS EC2 deployment process, including the EC2 instance, SSH connection, installed tools, project cloning, successful tests, and the application running on the AWS server.

**Proof of Work:**
[Google Drive – AWS EC2 Proof of Work](https://drive.google.com/drive/folders/1gO2KStI1NfabWLzmJjh31OPQIh-aFIiw?usp=drive_link)


## Verification

WTC-9UJBX2LR

## Project Status

The cloud deployment was completed and the application was successfully tested and run on an AWS EC2 Linux server.

