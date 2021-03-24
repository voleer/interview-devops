# Voleer DevOps Challenge

## Preface

This challenge is meant to see how you would approach a problem and not to see
how well you deliver a solution that we think is right. You should not focus on
getting _the_ "right" answer.

- The **#Instructions** below are general steps to get you started.

- The **#Questions** section has short-response questions to answer.

  For each question, you can answer it inline directly in the README.md in your forked repo.

- The **#Challenges** section has more open-ended problems for you to solve in
  any way you see fit.

  For each challenge listed below, you can propose your approach, it's always a
  bonus if you can execute your proposal. Some challenges are posted as open-ended
  questions and you can answer them inline.

  The challenges are estimated to take between **2 - 8 hours** depending on how familiar
  you are with containerization technology. Research time is also accounted for in the
  estimated duration.

## Instructions

1. Download this repo and, using this one as the base, create a new **private** repo.
2. Provide your answers in your generated repo.
3. Once your repo is ready for review, you can add `voleer-dev` user as a collaborator
   for your repo.
4. Wait for our response.

## Questions

### 1. What even is DevOps?

DevOps can mean different things depending on the company you work for or who you talk to.
At BitTitan, we believe that "**Principles and Mindset > Practices > Tools**".

- What is your take on the definition of DevOps?

- Why has DevOps gained so much prominence recently?

### 2. Testing philosophy

One aspect of writing code, whether it's in a scripting or programming language, is testing. Everyone seems to agree that it is important but not everyone does it.

- What is your personal testing philosophy and how do you test your code?

- What are some considerations to keep in mind when writing code with respect to testing?

### 3. Weapons of choice

There are so many tools available to us DevOps folks that it can be hard to keep up with all of them. Help us understand the weapons you choose to wield inside or outside of work.

- What is your primary OS?

- What shell do you use most often?

- Which scripting language(s) are you comfortable using? Which one is your favorite and why?

- Which programming language(s) are you comfortable using? Which one is your favorite and why?

- Which cloud provider(s) have you had experience with and what have you used them for?

- Name a few tools/applications that you use and describe their purpose in your work.

## Repo structure

The example application stack is a social blogging site (i.e. a Medium.com clone) called "Conduit". It uses a custom API for all requests, including authentication.

**In this repo, you will find:**

- [./api](./api):

  - API specification and some utilities to test the backend.

- [./src/frontend](./src/frontend):

  - Source code for frontend UI application using React.js. You can read more about it in [./src/frontend/README.md](./src/frontend/README.md).
  - Locally, the application runs on http://localhost:4100

- [./src/backend.v1](./src/backend.v1):

  - Source code for legacy backend server code. This is written in Golang, and you can read more about it in [./src/backend.v1/readme.md](./src/backend.v1/readme.md).
  - Locally, the application runs on http://localhost:8080

- [./src/backend.v2](./src/backend.v2):

  - Source code for new backend server code that we are still developing. This is written in .NET Core, and you can read more about it in [./src/backend.v2/readme.md](./src/backend.v2/readme.md).
  - Locally, the application runs on http://localhost:5000

## Challenges

The following challenges are related to the repo. To provide your take on the
challenges, remember to commit your answers to your repo.

### 1. Can we Containerize these services?

We have heard good things about containerization technology, and think what if
we bring in to our application stack. Can you help Containerize the `frontend`, `backend.v1` and `backend.v2`?

We have provided a basic `Dockerfile` in each service's folder to help you get started.

### 2. Can we automate the container build?

Currently, our developers have to manually run `docker build` after they make changes. Can you write a script to
automate the build process and start a new container with the updated image?

### 3. Have you heard of that Kubernetes thing?

[Kubernetes](https://kubernetes.io/) seems like a great tool to help us with deploying, scaling, and managing these containerized services.

Can you create a `yaml` file for each service with the necessary Kubernetes resources that will allow us to scale them out in the future?

### 4. (Extra) Ship it.

Infrastructure as code (IaC) is really popular.

- How is it related to Kubernetes?
- Would IaC help us? If it would, how do we apply it to our stack?

**Nice to have:** It would be a super cool demo to our stakeholders if we can get the applications online and they can access it from their computer.
It's okay if it's a just an IP address or some random domain name.

If you want to take up this challenge. Please send an email to us and we will provide you
with a limited access to a Kubernetes cluster that you can deploy the applications there. But if you have your own solution, go for it.
