## Context

As high school kids enduring online school during pandemic we’ve felt the repercussions both mentally and physically. Sitting in front of a computer for extended amounts of time can cause pain in both the back and neck. Furthermore, it can be hard to focus with the lack of motivation that comes as a result of online school. 

## How It Works

Alert.AI uses a posture machine learning model and eye recognition machine learning model in tandem with a scoring system that outputs a score out of a 100 to a teacher on how attentive each of their students are. In addition, graphs are given for each student, allowing for a graphical representation that shows the progression of engagement over a class period. On the student end, they are given reminders during class to pay attention when our machine learning model recognizes that they aren’t engaged through their posture. Concurrently, the model will allow students to be more alert about their posture to help prevent long-term effects of back and neck pain-two prevalent causes of stress.

## Run With Docker

This method is easier, but can be less ideal for development depending on your specific setup. On a Windows computer, you will not be able to hot reload the code, meaning code changes will not be immediately reflected upon saving the file. This is not an issue on macs.

However, using the docker environment will allow you to run all the different parts of the app with one command. Although the routing will probably be configured for the other environment because I'm doing most of the dev on a windows computer...

### Step 1

Install [DockerDesktop](https://www.docker.com/products/docker-desktop). Follow all instructions then continue to step 2.

### Step 2

From the root of the repository, run `docker-compose up`

This should build the different images and run them in one environment. If you are one a mac, code changes will be reflected (at least in the React App, haven't set up nodemon for Express) upon save (hot reload). If not, you will have to close the environment with 'docker-compose down' or exit the process with Ctrl+C in the terminal (VSCode Powershell). Can also be stopped from docker desktop.
