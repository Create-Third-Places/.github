# Development


The goal of this project is to build a non commercial open source platform to help people organize and host in person events. The backend will also have an open API that other specialized websites can use to list and manage events.


As a starting point, the project has a site specific for board games in the Washington, DC area, https://dmvboardgames.com/.


For a list of issues recommended for first time contributors, look [here](https://github.com/Create-Third-Places/DMVBoardGames/issues?q=is%3Aissue%20state%3Aopen%20label%3A%22good%20first%20issue%22). Issues will have a point value indicating the estimated complexity.


# Repos

- [development](https://github.com/Create-Third-Places/development): Documentation and scripts for development.
- [backend](https://github.com/Create-Third-Places/backend): Backend APIs.
- [database](https://github.com/Create-Third-Places/database): Scripts related to the database.
- [DMVBoardGames](https://github.com/Create-Third-Places/DMVBoardGames): Website for in person board game events in the DC area. It will use the backend APIs of this project.
- [user-management](https://github.com/Create-Third-Places/user-management): Logic related to authentication, authorization, and managing users. This includes actions related to creating or deleting data that can only be modified by certain users.
# Tech stack
- Vanilla JavaScript on the UI. The UI might be moved to use a library or framework besides React.
- Vanilla CSS.
- PostgreSQL
- Java

# Development guidelines

## Development proccess
- Post a comment on an issue indicating that you want to start working on it.
- Once the issue is assigned to you, and you are finished with a code change for the issue, create a PR to the main branch. If a feature is complex, split up the work into mupltiple smaller PRs if possible.
- When creating a PR, include a description of the change.
- Once a PR has passed the review, a maintainer will approve and merge it.

## Development guidelines
- If you are working on a change related to an issue, keep the changes limited to the scope of the issue. If you think it makes sense to update the scope, post a comment on the issue.
- All code for a feature must be written by a developer. Code written by ChatGPT, GitHub Copilot, Claude Sonnet, or any other generative AI tool cannot be used to write code. Also, AI should not be used to support any website functionality such as a group search.
- If you want to introduce a new technology not listed as part of the tech stack, email gulu@createthirdplaces.com. Include details about the technology and why you think it would be useful. If it is determined that the technology is relevant, you will get a reply back indicating that it can be used.
- All communication with the backend will be done through API endpoints implemented in the backend repo.

# Suggesting changes
If you have a recommendation for a new feature, enhancment, or bug fix, create an issue in the development repo. Make sure any issues created follow these guidelines.
- All code should be written by a developer without the use of generative AI tools such as ChatGPT or GitHub Copilot. The  feature should also not be dependent on generative AI or machine learning tools.
- All changes must support the goal of encouraging people to interact in person.  On the other hand, a feature that makes it easier for people to find in person social events would be a good fit for the website. Changes to improve usability or readability of the website are also encouraged.


# Guidelines for architecture

## Decoupling
Decoupling different parts of the application is important to maintain flexibility in the technolgies we use. There are many factors determining the technologies we should use, and we can't predict all of them in advance. 

It is possible that users may ask for a feature that isn't supported by the technolgy that is used, or it is determined that a technology used does not make sense with the scalability requirements. There might also be some roadblock we discover.

It is possible that users may ask for a feature that is not supported 
