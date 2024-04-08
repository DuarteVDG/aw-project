# `Statistics` Micro-Frontend

## Description

The `Statistics` micro-frontend is dedicated to displaying both positive and negative statistics related to meat-associated topics. Its purpose is to promote user awareness.

## Justification
- **Simplicity & Single Responsibility:** This micro-frontend has a clear purpose of presenting statistical data related to meat topics, avoiding unnecessary complexity.
- **Reusability & Flexibility:** Allows for easy adaptation to changing requirements or additional statistical data sources without significant impact on the overall application.
- **Independent Deployment & Autonomous Teams:** Can be deployed independently of micro-frontends within the application, facilitating development and maintenance.

## Responsabilities
- Provide a user-friendly interface for browsing and exploring different statistics.
- Display positive and negative statistics related to meat production, consumption, and related topics.
- Promote user awareness regarding meat related topics.

## Consequences and Implications
- **Positive:** Provides informative statistics, promoting transparency and awareness, and optimizes user experience
- **Negative:** May increase app overhead and/or present controversial statistics.

## Notes
As the app is currently designed and implemented, the only way to access the `Statistics` micro-frontend is through a button in the `News` micro-frontend. However this should be altered to allow users to access `Statistics` without having to go through the `News`, considering users may be interested in only one of these sections. Thus, we opted to implement both of these micro-frontends separated.

## Views
<div style="text-align: center;">
     <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/micro-frontends/images/Statistics3.png?raw=true" style="width: 200px; height: auto;">
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/micro-frontends/images/Statistics1.png?raw=true" style="width: 200px; height: auto;">
    <img src="https://github.com/DuarteVDG/aw-project/blob/main/front-end/micro-frontends/images/Statistics2.png?raw=true" style="width: 200px; height: auto;">
</div>
