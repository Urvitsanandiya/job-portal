# Job Portal

Job portal with two roles: Employer and Applicant.

## Overview
Minimal job portal. Secure authentication. Applicants build profiles and apply for jobs. Employers post jobs and manage applicants. Notifications for major events. Responsive UI built with React and Tailwind CSS.

## Tech Stack
- Backend: Spring Boot with role-based access  
- Auth: JWT (optional), password hashing, OTP-based reset  
- Database: MongoDB  
- Frontend: React + Tailwind CSS  

## Backend — Setup
1. Clone the repository  
2. Enter backend folder  
3. Install dependencies  
   ```bash
   mvn clean package -DskipTests
   ```
4. Run locally  
   ```bash
   java -jar target/job-portal-backend.jar
   ```
5. Or run in dev  
   ```bash
   mvn spring-boot:run
   ```

## Frontend — Setup
1. Enter frontend folder  
2. Install packages  
   ```bash
   npm install
   ```
3. Start development server  
   ```bash
   npm start
   ```
4. Build for production  
   ```bash
   npm run build
   ```

## Features — Linear Flow
1. User signs up and verifies. Password hashed.  
2. User logs in. Server issues JWT if enabled.  
3. Applicant completes profile with photo and skills.  
4. Applicant searches jobs using filters: title, location, experience, job type, salary.  
5. Applicant sorts results by relevance or salary.  
6. Applicant views job details and applies or saves. Application saved. Notification created.  
7. Applicant views other developer profiles.  
8. Applicant tracks status: saved → applied → interviewing → offered.  
9. Employer posts jobs. Employers edit or delete jobs.  
10. Employer views applicants. Employers view profiles.  
11. Employer schedules interviews and updates application status. Notifications generated.  
12. Users can clear notifications.

## Folder Structure
```
/backend
  /src
    /main/java/...controllers
                 ...services
                 ...repositories
  pom.xml

/frontend
  /src/components
  /src/pages
  package.json
