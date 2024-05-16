## Context

This project addresses a challenge faced by online educators: maintaining student attentiveness during virtual lectures.  Traditional online learning environments can struggle to replicate the focus and interaction found in physical classrooms. This can lead to decreased engagement and ultimately hinder learning outcomes.

## How It Works

This platform aims to improve student focus and participation in online lectures by incorporating the following features:

- Real-time Attention Monitoring: The platform utilizes posture and eye recognition models, built using Keras, to assess student engagement during lectures.
- Engagement Prompts: Based on the attention models, real-time reminders are delivered to students when needed, prompting them to re-engage with the material.
- Gamification: A gamified scoring system motivates students to stay focused and participate.
- Engagement Visualization: Line graphs provide instructors with a visual representation of student engagement throughout the lecture, allowing them to adapt their teaching approach if needed.

This combination of features creates a more interactive learning environment that encourages student participation and improves overall engagement.

## Run With Docker

While Docker offers a streamlined way to run the application, it might not be the most convenient choice for active development, depending on your setup. Here's why:

- Hot Reloading: On Windows with Docker, code changes won't be automatically reflected (hot reload) like they might be on macOS. This means you'll need to rebuild and restart the container after every modification.
However, Docker excels at running all application components with a single command, making it a great option for deployment.

Here's how to get started with Docker development:

- Install Docker Desktop: Head over to Docker Desktop and follow the installation instructions.

- Run the Application: Once Docker is set up, navigate to the project's root directory in your terminal and execute docker-compose up. This command will build the necessary Docker images and launch them as a single environment.

Hot Reload Note: Currently, hot reload functionality is likely only available for the React app on macOS. For other environments or operating systems, you'll need to rebuild and restart the container after making code changes. You can stop the environment using docker-compose down in the terminal or through Docker Desktop.
