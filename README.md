# Smart India Hackathon Workshop
# Date:26.02.2025
## Register Number:212224040348
## Name:TAMILSELVI I
## Problem Title
SIH 1653: Web based Selector-Applicant Simulation Software
## Problem Description
Background: Recruitment and Assessment Centre (RAC) under DRDO, Ministry of Defence carries out interviews for applications received against advertised vacancies and for promotion to next higher grade for scientific manpower inducted within DRDO. Description: The process of interviewing is a challenging task. An unbiased objective interviewing process helps identify the right talent. The basic process of an interview involves posing a set of questions by an interviewer and thereafter evaluating responses from candidates. Thus, the questions asked should be relevant and match the area/ expertise of the applicant and the responses should also be of relevance w.r.t. the question asked. Expected Solution: The proposed solution should provide experts as well as candidates a real life Board Room experience, starting with initial ice-breaking questions leading to in-depth techno-managerial (depending on the level of candidate) questions. It shall also be able to provide a quantifiable score for experts as well as the candidate for the relevancy of questions w.r.t. the area/ expertise of the applicant. Similarly, candidate responses should also be graded for relevancy w.r.t. the question asked, finally assisting in arriving at an overall score for the subject knowledge of the candidate and thus his/ her suitability against the advertised post.

## Problem Creater's Organization
Ministry of Defence

## Idea
```
1. Environment-focused Recruitment Simulation:
Idea: Develop a simulation platform that allows the Ministry of Environment to assess applicants for various positions based on their knowledge and skills related to environmental policies, sustainability practices, and ecological challenges. This platform could simulate real-world scenarios like climate change negotiations, policy-making for conservation, or crisis management during environmental disasters.
Features:
Virtual scenarios like disaster response or policy development
Decision-making simulations related to environmental laws, regulations, and enforcement
Real-time feedback for applicants based on their responses and decisions
AI-driven grading system for evaluating technical knowledge and problem-solving skills
2. Environmental Awareness & Education Portal for Applicants:
Idea: A web-based platform could be developed to educate potential employees on the Ministry's objectives, policies, and current environmental challenges. The platform can have interactive modules where applicants can test their knowledge about ronmental policy-making
3. Environmental Impact Evaluation Simulation for Applicants:
Idea: A simulation tool that allows applicants to demonstrate their ability to evaluate the environmental impact of various industrial, construction, or development projects. This could help assess how well applicants can apply knowledge of environmental regulations to real-world situations.
Features:
Virtual simulations of industrial development projects (e.g., dams, factories, urban development)
Applicants must evaluate the impact on air, water, and biodiversity, providing mitigation strategies
AI tools to score and suggest improvements for applicants' solutions
4. Sustainability Leadership Simulation:
Idea: This could be a simulation for assessing leadership qualities of applicants who are being considered for leadership roles within the Ministry. The focus would be on managing large-scale environmental projects or leading sustainability initiatives.
Features:
Situational decision-making challenges based on global environmental crises
Crisis management tasks (e.g., pollution spill, habitat destruction)
Evaluating applicants' ability to work under pressure, collaborate, and lead teams towards sustainable solutions
5. Real-time Collaboration Simulation for Multi-Stakeholder Environmental Negotiations:
Idea: A simulation tool where applicants can participate in environmental policy negotiations involving multiple stakeholders—government, NGOs, industry, and communities—to tackle a pressing environmental issue like deforestation, marine pollution, or climate change.
```

## Proposed Solution / Architecture Diagram



![Screenshot 2025-02-26 120913](https://github.com/user-attachments/assets/c62463ea-ccdc-401d-845b-83e1fbdb7916)



## Use Cases



![image](https://github.com/user-attachments/assets/7bb27047-08e9-45bd-aea0-886e9748d8ff)



## Technology Stack
1. Frontend (User Interface)
The frontend should provide a seamless, interactive, and user-friendly interface where applicants can engage with the simulation scenarios, input decisions, and view feedback.

Frameworks/Tools:

React or Vue.js: For building a dynamic and responsive user interface. React is especially popular for handling complex user interfaces and real-time updates, making it ideal for simulation-based interactions.
Redux (for React) or Vuex (for Vue.js): For state management across the application, ensuring smooth interactions across different components.
Bootstrap or Material-UI: For responsive, pre-styled UI components that can speed up the development process and ensure mobile-first design.
Languages:

JavaScript/TypeScript: JavaScript is the primary language for frontend development. TypeScript can also be used for better type safety, especially in complex applications.
Styling:

Sass/SCSS or Styled Components: For writing modular and maintainable CSS.
2. Backend (Server-side and Simulation Logic)
The backend will handle user authentication, scenario logic, real-time scoring, data processing, and simulation management.

Frameworks/Tools:

Node.js with Express.js: Node.js provides an asynchronous, event-driven framework for handling requests, and Express.js is lightweight and easy to use for RESTful APIs and backend services.
Python with Flask or Django: For simulation-heavy backends. Python is commonly used in AI and machine learning applications, and frameworks like Flask or Django are easy to set up for handling business logic and data manipulation.
Simulation Engine:

JavaScript (Node.js) or Python can be used to implement the simulation logic and real-time decision-making scenarios. Python, with its libraries (e.g., Pandas, NumPy), could be used for environmental data processing and scoring mechanisms.
Real-time Communication:

Socket.io (Node.js): For real-time interaction in simulations, where multiple decision points need to be updated live without reloading the page.
WebSockets: For live communication between the server and the frontend to simulate a real-time environment and give instant feedback during the simulation.
Data Processing:

AI & Machine Learning Libraries (optional, depending on complexity):
Scikit-learn, TensorFlow, or PyTorch for scoring algorithms or evaluation models that could assess applicant performance on various environmental scenarios.
Natural Language Processing (NLP) libraries (e.g., spaCy, NLTK) for analyzing text-based responses if the simulation requires open-ended feedback.
3. Database (Data Storage)
The database will store applicant data, simulation scenarios, user progress, decision logs, feedback reports, and other critical data.

Relational Databases:

PostgreSQL: A powerful, open-source relational database suitable for structured data, such as user profiles, simulation results, feedback, and logs.
MySQL: Another option for relational databases, commonly used for web applications.
Non-relational Databases (Optional):

MongoDB: If you need flexibility in data storage, especially when storing unstructured data or logs, MongoDB can store documents in JSON format.
Cloud-Based Databases (optional):

Amazon RDS: Managed database service for PostgreSQL or MySQL.
Firebase: For faster prototyping and if real-time data synchronization is required.
4. Authentication and Security
User authentication, access control, and security are crucial to protect applicants' data and ensure integrity during the simulation process.

Authentication:

OAuth 2.0 with JWT (JSON Web Tokens): For secure, token-based authentication to authenticate users and authorize their access to the system.
Passport.js (for Node.js) or Django-Allauth (for Django) to handle user authentication flows.
Encryption:

SSL/TLS: Secure Sockets Layer (SSL) encryption for secure communication between the client and the server.
bcrypt: For securely hashing passwords.
Authorization:

Role-based access control (RBAC) to differentiate between applicants, hiring managers, and system administrators, each having different access permissions.
5. Cloud Infrastructure and Hosting
The application should be hosted on a cloud infrastructure to ensure scalability, security, and easy maintenance.

Cloud Services:

AWS (Amazon Web Services): Services like EC2 (for compute instances), S3 (for storage), Lambda (for serverless functions), and RDS (for database management) can be used to host the application.
Azure or Google Cloud: Other alternatives for cloud hosting services with similar offerings.
CI/CD Pipeline:

GitHub Actions, GitLab CI, or Jenkins: To automate testing and deployment pipelines. Ensures code is automatically deployed and tested as new changes are made.
6. Analytics and Reporting
To evaluate and generate reports on the applicant's performance during the simulation:

Data Analytics:

Python (Pandas, NumPy) for analyzing simulation data and creating detailed reports based on applicant performance.
Google Analytics or Mixpanel (optional) to track user interactions within the platform.
Report Generation:

PDF Libraries (e.g., jsPDF for JavaScript or ReportLab for Python) for generating downloadable reports based on applicant performance in the simulation.
Data visualization libraries like D3.js or Chart.js to provide graphical insights into the applicant’s decision-making process (e.g., visualizing environmental impact scores, stakeholder satisfaction, etc.).
7. Testing
For ensuring that the software is reliable, secure, and performs well under load:

Unit Testing Frameworks:

Jest (for JavaScript/React)
Mocha/Chai (for Node.js)
PyTest (for Python-based testing)
End-to-End Testing:

Cypress or Selenium: To perform automated end-to-end testing for the simulation’s interactions.
Load Testing:

JMeter or Artillery: To simulate multiple users accessing the system concurrently and measure performance.
8. Deployment
The deployment process should be simple and scalable to handle growing traffic and ensure uptime.

Containerization:
Docker: To package the application into containers for consistent deployment across different environments (e.g., development, staging, production).
Container Orchestration:
Kubernetes: For managing and scaling the Docker containers in a cloud environment, ensuring high availability and resource optimization.
Summary of the Technology Stack:
Frontend:

React or Vue.js
Redux/Vuex
Material-UI/Bootstrap
JavaScript/TypeScript
Sass/Styled Components
Backend:

Node.js with Express or Python with Flask/Django
Socket.io or WebSockets
Python Libraries (Scikit-learn, Pandas, NumPy)
JWT for authentication
Database:

PostgreSQL or MySQL
MongoDB (optional)
AWS RDS/Firebase (for cloud databases)
Authentication/Security:

OAuth 2.0, JWT
bcrypt
SSL/TLS Encryption
Cloud Infrastructure:

AWS, Google Cloud, or Azure
GitHub Actions/Jenkins for CI/CD
Analytics & Reporting:

Python (Pandas, NumPy) for analytics
jsPDF or ReportLab for report generation
D3.js/Chart.js for data visualization
Testing:

Jest, Mocha/Chai, PyTest for unit testing
Cypress/Selenium for E2E testing
Deployment:

Docker for containerization
Kubernetes for orchestration



## Dependencies:
1. Frontend Dependencies
Core Libraries
React (or Vue.js if using Vue):

react - The core React library.
react-dom - For rendering React components in the DOM.
react-router-dom - For handling routing and navigation within the React app.
2. Backend Dependencies
Core Libraries & Frameworks
Node.js with Express (if using Node.js for the backend):

express - A fast and lightweight Node.js web framework for handling HTTP requests and routing.
cors - For enabling Cross-Origin Resource Sharing (CORS) when your frontend and backend are served from different origins.
body-parser - For parsing incoming request bodies.


