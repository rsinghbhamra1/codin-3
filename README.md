# Coding Assignment 13 - UC Component Library 

This project is a **React web component library** built using **Storybook**. It contains reusable UI components that you can easily develop, test, and document. These components are meant to be used in real-world React applications. They are flexible and help keep your projects consistent and easy to maintain.

To keep the code clean and error-free, the project uses **Husky** for pre-commit checks, running automated checks for code formatting, linting, and testing. It also uses **GitHub Actions** to automatically enforce code quality on every push or pull request.

## Components Overview

The project includes the following React components:

1. **Button**: A customizable button component.
2. **Card**: A card layout component to display content.
3. **Dropdown**: A dropdown menu for selection inputs.
4. **HeroImage**: A large image component often used in hero sections.
5. **Img**: A basic image component for displaying images.
6. **Label**: A label component for forms and other UI elements.
7. **RadioButton**: A radio button component for form selections.
8. **Table**: A table component for displaying data.
9. **Text**: A basic text component for paragraphs and more.

# Pre-commit Tests
* Prettier
* EsLint 
* Tests 

## Getting Started

To get the project running locally on `localhost:8018`, follow the steps below.

### Prerequisites

Make sure you have:

- [Git](https://git-scm.com/downloads)
- [Docker](https://www.docker.com/get-started)

### Instructions

1. **Clone the repository**

   Pull the project repository:

   ```bash
   git pull https://github.com/rsinghbhamra1/codin-3.git
   ```

2. **Build the Docker image**

   Navigate to the project folder and build the Docker image:

   ```bash
   docker build -t bhamra_rupinderjit_coding_assignment13 .
   ```

3. **Run the Docker container**

   Run the container on port `8018`:

   ```bash
   docker run -d -p 8018:8018 --name coding_assignment13_storybook bhamra_rupinderjit_coding_assignment13:latest
   ```

4. **Access Storybook**

   Open Storybook in your browser:

   ```
   http://127.0.0.1:8018
   ```

   Here, you can view and test all the components.

### Stopping the Docker Container

To stop the container, run:

```bash
docker stop coding_assignment13_storybook
```

To remove the container after stopping it:

```bash
docker rm coding_assignment13_storybook
```

### Testing Github Pre-Commit

just make a test commit:

```bash
git commit -m "Husky test commit"
```
