# SafePlate
An Alexa skill that easily tells the user the health inspection score of a restaurant using the database provided by the SF government.

## Inspiration
We were inspired by the impact of big data on public health. We realized that there was a plethora of public health data that wasn't being fully utilized, so we wanted to create something that uses the large amount of available data to inform the public of public health issues that people normally don't think about.

## What it does
Our Alexa skill tells the user the health inspection score on any amazon device. Furthermore, the user can ask Alexa for the phone number of the restaurant if they are interested in giving them a ring!

## How we built it
### Backend
We developed a custom API that bridges the gap between our database in MongoDB and our frontend application that was hosted on Alexa. This API allowed us to make the most of our free tier subscriptions to the technologies that are at the core of our application by keeping the database private and decentralized, which makes our application scalable.
### Frontend
We developed an Alexa skill that utilized our custom API to query information that the user asks Alexa. We used AWS Lambda to serve as the middleware that extracted speech information from the user, retrieved information from our API, and presented the retrieved information to the user.

## Challenges we ran into
We had planned to use Node and JavaScript as our primary technologies to build our application, but we ran into issues that we did not know how to solve, so we switched to Python. Additionally, we switched from a website to display our application to an Alexa skill because we ran into issues in having our website communicate with our backend API because the network blocked access to our API.

## Accomplishments that we're proud of
We accomplished a working product. We developed a full stack application that had a database, an API that connected the database with the Alexa skill, and a working demo of our skill on Alexa. We are especially proud that we were able to demo our application without having to hardcode all components of our application.

## What we learned
JavaScript is especially hard to use if you have little to zero experience. We also learned how to develop an Alexa skill using AWS services.

## What's next for SafePlate
Our immediate goal is to scale our application by deploying our publicly accessible API on a cloud service. We also would like to implement more features into Alexa to make her more intuitive to use and better accessible for people of all ages.
