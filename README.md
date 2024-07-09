# Discord Job Listings Bot

Welcome to the **Discord Job Listings Bot** repository! This bot is designed to help members of the UF NSBE (University of Florida's National Society of Black Engineers) stay updated with the latest internship and new grad opportunities from the SimplifyJobs organization.

![image](https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/42ae85cf-4a4a-4af3-be58-0109822e166e)


## Overview

I love supporting my peers by providing tools and resources that enhance our journey as engineers. This bot ensures that every member is aware of new opportunities as they arise, thanks to the SimplifyJobs organization.

<img width="431" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/5d25437a-47d0-470a-9edd-5bdb86483754">

[Join here](https://discord.gg/BD26qHZ7Yr)

## How It Works

The bot automatically scans for new internship and new grad roles from the SimplifyJobs organization and posts them directly to the `#career-opportunities` channel on our UF NSBE Discord server. This way, members can stay informed about the latest opportunities without having to search for them manually.

## Features

- **Real-time Job Updates**: Internship and new grad listings are posted as soon as they are available.
- **Focused on Members**: Tailored specifically for the UF NSBE community to help everyone become better engineers and find success, thanks to SimplifyJobs.

## Why This Matters

In April 2024, I had the honor to be inducted and officially represent my local chapter as President. I work to be the backbone and reinforcement for my peers. This bot is a step towards that goal, making sure that every member has the best chance to succeed by staying informed about career opportunities. With SimplifyJobs providing these listings, we're ensuring you have access to some of the best opportunities out there.

## How to Recreate This Bot in Your Discord Channel

### Step 1: Create Your Own Discord Bot

1. **Go to the Discord Developer Portal**: Visit [Discord Developer Portal](https://discord.com/developers/applications).
2. **Create a New Application**: Click on "New Application" and give it a name.
  
<img width="732" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/c06c5477-66a1-44c7-914b-afdafeed8910">

### Step 2: Add Your Bot to Your Discord Server

1. **Get the OAuth2 URL**: Under the "OAuth2" tab, select the bot scope and permissions your bot needs. Generate the URL.
   
<img width="935" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/8649acb4-b133-4b87-8e33-68dffafdbb18">

2. **Invite the Bot**: Use the generated URL to invite the bot to your Discord server.
   
<img width="403" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/239e1483-22c4-470f-bb27-a38b271cb637">


### Step 3: Set Up a Discord Webhook

1. **Create a Webhook**: In your Discord server, go to the channel where you want job listings posted. Under "Integrations", create a new webhook.
   
<img width="486" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/f76dbcdf-51cd-4251-a214-6a4a6a630e72">

2. **Copy the Webhook URL**: Save this URL as you will need it for the bot to send messages.
   
<img width="498" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/9c80a975-fc36-4719-98b9-b4cd19eb6693">


### Step 4: Personal Access Token on GitHub

1. **Generate a Personal Access Token**: Go to your GitHub settings, navigate to "Developer settings", and then "Personal access tokens". Generate a new token with appropriate permissions.
   
<img width="495" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/f68aa82f-a0e2-4028-b15c-4e73b772fdc7">

2. **Add Token to GitHub Secrets**: In your repository, go to "Settings" > "Secrets" and add your token as `PERSONAL_ACCESS_TOKEN`.
   
<img width="689" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/bb1d6941-f4b2-456f-b30f-82db273088de">


### Step 5: Set Up the Repository

1. **Clone the Repository**: Clone this repository to your local machine.
   
<img width="364" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/6bd87b9a-5628-4782-b9c6-56dfb464d4c5">

2. **Configure the Environment Variables**: Set up your `.env` file or configure your secrets in GitHub Actions to include `DISCORD_WEBHOOK` (Copy paste your discord webhook link to the 'value' space).
   
<img width="443" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/ab736e68-360a-45bf-aa40-8b158a0bc6f7">


### Step 6: Automate the Workflow with GitHub Actions

1. **Create GitHub Actions**: Use the provided workflow files in the `.github/workflows` directory to automate job listing checks and Discord notifications.
   
<img width="764" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/8c6e574d-b37f-4296-95f5-4bd7d3e4b6c0">

2. **Customize the Bot to your liking**: Modify the scripts as needed to fit your specific requirements (refer to the listings.json scripts in SimplyJobs Organizations for proper extraction of stored variables).
   
<img width="428" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/3941da7f-a71f-4dd6-8e6a-04e6a4ff8015">


<img width="233" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/bfa2379a-8da7-4bb3-8b9d-6ecc29353df9">



### Step 7: Deploy and Test

1. **Deploy the Bot**: Push your changes to GitHub to trigger the GitHub Actions workflows.
   
<img width="945" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/1daeba39-ea13-44b3-a765-6e559e945511">

2. **Test the Bot**: Ensure the bot is posting job listings correctly in your specified Discord channel.
   
<img width="352" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/cfda7531-520c-43a8-ac1b-8cac8306c4d9">


### Giving Credit

We want to give a big shout-out to [SimplifyJobs](https://simplify.jobs) for providing the internship and new grad listings that power this bot. Their platform curates top-notch opportunities, and we are grateful for their work and dedication. By using these listings, we ensure our members have access to some of the best job opportunities available. Thank you, SimplifyJobs!

![image](https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/9e346daf-4b1a-4b40-bedc-171f91d6e13f)

