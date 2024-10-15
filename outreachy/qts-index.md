# QuickStatements 3.0 Home's Page

**QuickStatements 3.0 Home's Page** allows for the editing of adding new batches, viewing batch details, and accessing batches submitted by users. It does this through simple set of text commands. 

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Makefile Commands](#makefile-commands)
- [Contributing](#contributing)
- [Support](#license)

## Features

### Navigation Bar 
The following are available on the navigation are:
- **New Batch**: This enables new batch of statements in Wikimedia projects.
- **Last Batches**: This enables viewing existing batches.
- **Git**: This provides the users with access to the source code repository, should they want to contribute to the codebase of QuickStatements.

### Homepage Overview
The following features are available on QuickStatements home page:
- **New batch button**: This button allows a user to create a new set of batch statements.
- **Batch ID Search**: This search feature enables a user to enter an ID to retrieve the details of a specific batch.
- **Username Search**: This search feature makes access of batches by a particular user possible.
- **Login**: The login feature allows users to log into the website so as to create and/or manage their batches. 

## Installation

### Prerequisites
- **Docker**: Docker must be installed and running on your machine. For Windows users, WSL2 (Windows Subsystem for Linux) must be integrated with the Docker desktop.
- **Make**: Make must also be installed, as it is needed to run the tasks defined in the Makefile.

### Steps
1. Clone the repository and change directory to the root folder of the project:
   ```bash
   git clone https://github.com/DevUju/qts3-wmb-test.git
   cd qts3-wmb-test
   ```

2. Build the Docker image:
   ```bash
   make build
   ```

3. Start the container and enter the shell:
   ```bash
   make shell
   ```

4. Run the application inside the Docker container:
   ```bash
   make run
   ```

The application is accessible at:
```
http://localhost:8765
```

### Environment Setup
Place the `env` file in the `etc/env` directory, and set up your environment variables using `etc/env.SAMPLE` as a guide. 

## Usage

### Creating a New Batch
1. Click on the "New batch" button.
2. Fill the form.
3. Click on "Execute" to submit.

### Searching by Batch ID
1. Enter a valid batch ID.
2. Click "See batch details" to retrieve batch information.

### Searching by Username
1. Enter a username.
2. Click "See batches by user" to access all batches created by the user or associated with the username.

### Logging In
A user must log in to access the full functionality of QuikStatements, especially in relation to creating and managing batches.

## Makefile Commands
The project also includes a Makefile which manages the following commands:

- **make build**: Builds Docker image.
- **make shell**: Runs and accesses the Docker container in an interactive shell.
- **make run**: Start the QuickStatements application inside the Docker container.

## Contributing
To contribute to QuickStatements, do the following: 
1. Fork the project https://github.com/WikiMovimentoBrasil/qts3-wmb-test.
2. Clone the source code in your computer

## Support
If you have any question about the project or there are modifications that you would want to implement, kindly open an issue on the repository.
