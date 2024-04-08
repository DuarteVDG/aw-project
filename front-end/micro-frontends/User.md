# `User` Micro-Frontend

## Description

The `User` micro-frontend is responsible for handling all user-related aspects within the application, specifically authentication, profile management, and account settings.

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
- Allow users to give their feedback regarding different aspects of the application, such as the meat products.

## Consequences and Implications
- **Positive:** Enhances user security by managing authentication and authorization securely, whilst enhancing user experience by providing easy-to-use interfaces for login, registration, and password recovery, as well as personalized experience through profile management and saved products features.
- **Negative:** Potential downtime or issues with authentication could disrupt user access to the application and/or lead to security vulnerabilities within the application. Thus, may require intensive testing and maintenance efforts.

## Views
<div>
<img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/micro-frontends/images/UserAuthentication.png?raw=true" style="width: 200px; height: auto;">
<img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/micro-frontends/images/UserProfile1.png?raw=true" style="width: 200px; height: auto;">
<img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/micro-frontends/images/UserProfile3.png?raw=true" style="width: 200px; height: auto;">
<img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/micro-frontends/images/UserProfile2.png?raw=true" style="width: 200px; height: auto;">
<img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/micro-frontends/images/Feedback1.png?raw=true" style="width: 200px; height: auto;">
<img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/micro-frontends/images/Feedback2.png?raw=true" style="width: 200px; height: auto;">
</div>
  
