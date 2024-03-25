# `User` Micro-Frontend

## Description

The `User` micro-frontend is responsible for handling all user-related aspects within the application, specifically user authentication user profile management, and account settings.

## Justification
- **Simplicity & Single Responsibility:** Ensures simplicity by focusing on user-related functionalities, including authentication, profile management, and account settings.
- **Autonomous Teams and Independent Deployment:** This micro-frontend can be developed separately, allowing for independent updates and flexibility in the developing process.

## Responsabilities
- Provide interfaces for user login, registration, and password recovery.
- Manage user authentication and authorization processes.
- Maintain user sessions and handle authentication-related events.
- Provide access to account settings, including preferences and communication settings.
- Allow users to view and edit their profile information.
- Enable users to contact support or other users within the app.
- Allow users to log out of their current session.
- Implement the ability for users to save products and view their saved items.

## Consequences and Implications
- **Positive:** Enhances user security by managing authentication and authorization securely. Simplifies user experience by providing easy-to-use interfaces for login, registration, and password recovery.
Provides personalized experience through profile management and saved products features. Improves user engagement and retention by allowing customization of account settings and easy navigation.
- **Negative:** Potential downtime or issues with authentication could disrupt user access to the application and/or lead to security vulnerabilities within the application.Thus, may require intensive testing and maintenance efforts.

## Views
<div>
<img src="https://github.com/DuarteVDG/aw-project/blob/main/micro-frontends/images/UserAuthentication.png?raw=true" style="width: 200px; height: auto;">
<img src="https://github.com/DuarteVDG/aw-project/blob/main/micro-frontends/images/UserProfile1.png?raw=true" style="width: 200px; height: auto;">
<img src="https://github.com/DuarteVDG/aw-project/blob/main/micro-frontends/images/UserProfile3.png?raw=true" style="width: 200px; height: auto;">
<img src="https://github.com/DuarteVDG/aw-project/blob/main/micro-frontends/images/UserProfile2.png?raw=true" style="width: 200px; height: auto;">
</div>
  
