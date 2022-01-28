+++
title = "Tech Stack"
weight = 4
+++

{{<section title="Tech Stack">}}

#### Amazon AWS

During the early stages of our project we agreed that we want to run the application as costefficient, scalable and performant as possible. We therefore decided to build the system on a serverless architecture
using **[Amazon AWS Lambda functions](https://aws.amazon.com/de/lambda/)**. The lambda functions only run when they are called through their individual endpoints and provide the latest forecast data generated by the power consumption machine learning models.
This reduces the amount of computing power and completely minimizes the fixcosts required to run the application.
The forecastdata, as well as the entire frontend are stored on **[AWS S3 Buckets](https://aws.amazon.com/de/s3/)**.
The AWS environment enables us to add more resources like databases or mediastorage as required and when required.

#### React (Typescript) + Tailwindcss

Our frontend is built on **[React](https://reactjs.org/)** and **[Typescript](https://www.typescriptlang.org/)** which helped us to reduce bugs and unpredictable errors during development.
Typescript also makes it easier for future developers working on the project to dive into and understand the code and how our components work.
Using **[Tailwind Css](https://tailwindcss.com/)** and its utility first approach, we were able to rapidly build new components for our dashboard without having to spend too much time structuring our Css and thinking about methodlogies like **[BEM](http://getbem.com/introduction/)**.
{{</section>}}

{{<section title="Other Tools">}}

#### Gitlab

For hosting and versioning the project we used **Gitlab** which was provided by Exxeta.

Our CI/CD pipeline was built using **Gitlab CI** and includes a test stage, running when feature branches are merged into our development branch.
Whenever we completed a user story we merged our changes into our main branch which then triggers the build and deployment stage, building the application and deplyong it onto the AWS s3 Bucket.

#### Jira & Scrum

Our entire design and development process was strictly based on the **Scrum framework**. **Jira** helped us to manage our project and sprints.

#### Miro & Figma

For brainstorming, making notes during user interviews as well as tests, retros and meeting protocols we used **Miro**.
Our entire design was created using **Figma**.

#### Discord & Microsoft Teams

For internal meetings we used **Discord**, for external meetings with Exxeta and other stakeholders we used **Microsoft Teams**.
{{</section>}}