
![Screenshot 2023-09-04 at 11 19 21 AM](https://github.com/yashtyagi4/SuperFrog-Scheduler/assets/85970478/35fbad62-3099-4d7a-a1a2-c808dc8c7290)

**SuperFrog Scheduler:** A full-stack web application to enable user requests for TCU mascot, cheerleaders, and showgirls for private events.

<br>

## Implementation

- Developed a cohesive full-stack web application using MVVM and MVC patterns.
- Utilized Vue.js for front-end and Spring Boot for back-end infrastructure resulting in 20+ RESTful APIs.
- Data storage/retrieval with Spring Data JPA and H-2 Database Engine.
- Secure authentication and authorization mechanisms with Spring Security, JWT, and OAuth2.

<br>

## Demonstration

### Request App
https://github.com/yashtyagi4/SuperFrog-Scheduler/assets/85970478/a2758f03-5d14-40fd-803b-813d6fc7afd5

### Admin App
https://github.com/yashtyagi4/SuperFrog-Scheduler/assets/85970478/54f388a4-006e-49c3-882b-de67e6c59bdd



<br>

## Setup and Running the Project

### Backend Setup

1. Navigate to `SuperFrog-Scheduler/Backend/src/main/edu/tcu/cs/superfrogscheduler` inside the Spring application.
2. Run the file `SuperfrogSchedulerApplication` to activate all the APIs locally.

### Frontend Setup

#### RequestApp:

1. Navigate to `SuperFrog-Scheduler/Frontend/RequestApp`.
2. Install the required node modules using `npm install`.
3. Navigate to the `src` folder and run the application with `npm run dev`.

#### AdminApp:

1. Navigate to `SuperFrog-Scheduler/Frontend/AdminApp`.
2. Install the required node modules using `npm install`.
3. Navigate to the `src` folder and run the application with `npm run dev`.

After following the above steps, you will have three applications running on local hosts at different ports: the Backend project (Java/Spring) and two Frontend projects (AdminApp and RequestApp).

<br>

## Technologies Used

- JavaScript
- HTML
- CSS
- Vue.JS
- Java
- Spring Boot
- Spring Security
- H2 Database

<br>

## API Endpoints

### User APIs:

- **Add Superfrog User**: POST - `/api/v1/users`
- **Update User**: PUT - `/api/v1/users/{userId}`
- **Get User**: GET - `/api/v1/users/{userId}`
- **Get All Users**: GET - `/api/v1/users`
- **Assign User To Appearance**: POST - `/api/v1/users/assignments/{userId}/{requestId}`
- **Remove User From Appearance**: DELETE - `/api/v1/users/assignments/{userId}/{requestId}`
- **Get Current User**: GET - `/api/v1/users/me`
- **Update Current User Info**: PUT - `/api/v1/users/me`
- **Activate User**: POST - `/api/v1/users/active/{userId}`
- **Deactivate User**: POST - `/api/v1/users/inactive/{userId}`
- **Login User**: POST - `/api/v1/users/login`
- **Search Users By Criteria**: POST - `/api/v1/users/criteria`

### Appearance APIs:

- **Get Appearance**: GET - `/api/v1/appearances/{requestId}`
- **Add Appearance Request**: POST - `/api/v1/appearances`
- **Update Appearance**: PUT - `/api/v1/appearances/{requestId}`
- **Get All Appearances**: GET - `/api/v1/appearances`
- **Export Appearance Report (Excel)**: POST - `/api/v1/appearances/excel`
- **Approve Appearance Request**: POST - `/api/v1/appearances/approval/{requestId}`
- **Reject Appearance Request**: POST - `/api/v1/appearances/rejection/{requestId}`
- **Generate Payment Forms**: POST - `/api/v1/payment/payment-forms`
- **Mark Appearance as Complete**: POST - `/api/v1/appearances/complete/{requestId}`
- **Get Open Approved Appearance Requests**: GET - `/api/v1/appearances/approvals/open`
- **Cancel Appearance Request**: POST - `/api/v1/appearances/cancel/{requestId}`
- **Search Appearances By Criteria**: POST - `/api/v1/appearances/criteria`
- **Update Appearance (Spirit Director)**: PUT - `/api/v1/appearances/admin/{requestId}`
- **Get All Payment Forms**: GET - `/api/v1/payment/payment-forms`

<br>

## Frontend Dependencies

### AdminApp:

- **axios**: ^1.3.5
- **vue**: ^3.2.47
- **vue-router**: ^4.0.13

### RequestApp:

- **@googlemaps/js-api-loader**: ^1.15.1
- **axios**: ^1.4.0
- **sweetalert2**: ^11.7.3
- **vue**: ^3.2.47
- **vue-axios**: ^3.5.2
- **vue-router**: ^4.1.6
- **vue-sweetalert2**: ^5.0.5

<br>

## Backend Dependencies

- **Spring Data JPA**
    - Group: `org.springframework.boot`
    - Artifact: `spring-boot-starter-data-jpa`

- **Spring Web**
    - Group: `org.springframework.boot`
    - Artifact: `spring-boot-starter-web`

- **Jakarta Persistence API**
    - Group: `jakarta.persistence`
    - Artifact: `jakarta.persistence-api`
    - Version: `3.1.0`

- **Jakarta Validation API**
    - Group: `jakarta.validation`
    - Artifact: `jakarta.validation-api`
    - Version: `3.0.2`

- **Spring Boot Starter OAuth2 Resource Server**
    - Group: `org.springframework.boot`
    - Artifact: `spring-boot-starter-oauth2-resource-server`

- **Spring Security Test**
    - Group: `org.springframework.security`
    - Artifact: `spring-security-test`
    - Scope: `test`

- **Spring Boot Starter Security**
    - Group: `org.springframework.boot`
    - Artifact: `spring-boot-starter-security`
    - Version: `3.0.5`

- **Spring Boot Devtools**
    - Group: `org.springframework.boot`
    - Artifact: `spring-boot-devtools`
    - Scope: `runtime`

- **H2 Database**
    - Group: `com.h2database`
    - Artifact: `h2`
    - Scope: `runtime`

- **Spring Boot Starter Mail**
    - Group: `org.springframework.boot`
    - Artifact: `spring-boot-starter-mail`
    - Version: `3.0.5`

- **Spring Boot Starter Test**
    - Group: `org.springframework.boot`
    - Artifact: `spring-boot-starter-test`
    - Scope: `test`

- **Spring Boot Starter Validation**
    - Group: `org.springframework.boot`
    - Artifact: `spring-boot-starter-validation`

- **Apache POI**
    - Group: `org.apache.poi`
    - Artifact: `poi`
    - Version: `5.2.3`

- **Apache POI OOXML**
    - Group: `org.apache.poi`
    - Artifact: `poi-ooxml`
    - Version: `5.2.3`

- **Jakarta Servlet API**
    - Group: `jakarta.servlet`
    - Artifact: `jakarta.servlet-api`
    - Version: `6.0.0`
    - Scope: `provided`

- **OpenPDF**
    - Group: `com.github.librepdf`
    - Artifact: `openpdf`
    - Version: `1.3.30`

- **Apache PDFBox**
    - Group: `org.apache.pdfbox`
    - Artifact: `pdfbox`
    - Version: `2.0.28`
