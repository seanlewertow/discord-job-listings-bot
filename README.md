# Discord Job Listings Bot

Welcome to the **Discord Job Listings Bot** repository! This bot is designed to help members of the UF NSBE (University of Florida's National Society of Black Engineers) stay updated with the latest internship and new grad opportunities from the SimplifyJobs organization.

## Overview

As the President of UF NSBE, I am dedicated to supporting my peers by providing tools and resources that enhance our journey as engineers. This bot ensures that every member is aware of new opportunities as they arise, thanks to the SimplifyJobs organization.

## How It Works

The bot automatically scans for new internship and new grad roles from the SimplifyJobs organization and posts them directly to the `#career-opportunities` channel on our UF NSBE Discord server. This way, members can stay informed about the latest opportunities without having to search for them manually.

## Features

- **Real-time Job Updates**: Internship and new grad listings are posted as soon as they are available.
- **Focused on Members**: Tailored specifically for the UF NSBE community to help everyone become better engineers and find success, thanks to SimplifyJobs.

## Why This Matters

In my role as President, I strive to be the backbone and reinforcement for my peers. This bot is a step towards that goal, making sure that every member has the best chance to succeed by staying informed about career opportunities. With SimplifyJobs providing these listings, we're ensuring you have access to some of the best opportunities out there.

## How to Recreate This Bot in Your Discord Channel

### Step 1: Create Your Own Discord Bot

1. **Go to the Discord Developer Portal**: Visit [Discord Developer Portal](https://discord.com/developers/applications).
2. **Create a New Application**: Click on "New Application" and give it a name.
  <img width="732" alt="image" src="https://github.com/seanlewertow/discord-job-listings-bot/assets/116752300/c06c5477-66a1-44c7-914b-afdafeed8910">
3. **Create a Bot**: Navigate to the "Bot" tab and click "Add Bot". Confirm the creation.
   ![Create a Bot](https://example.com/screenshot3.png)

### Step 2: Add Your Bot to Your Discord Server

1. **Get the OAuth2 URL**: Under the "OAuth2" tab, select the bot scope and permissions your bot needs. Generate the URL.
   ![Get the OAuth2 URL](https://example.com/screenshot4.png)
2. **Invite the Bot**: Use the generated URL to invite the bot to your Discord server.
   ![Invite the Bot](https://example.com/screenshot5.png)

### Step 3: Set Up a Discord Webhook

1. **Create a Webhook**: In your Discord server, go to the channel where you want job listings posted. Under "Integrations", create a new webhook.
   ![Create a Webhook](https://example.com/screenshot6.png)
2. **Copy the Webhook URL**: Save this URL as you will need it for the bot to send messages.
   ![Copy the Webhook URL](https://example.com/screenshot7.png)

### Step 4: Personal Access Token on GitHub

1. **Generate a Personal Access Token**: Go to your GitHub settings, navigate to "Developer settings", and then "Personal access tokens". Generate a new token with appropriate permissions.
   ![Generate a Personal Access Token](https://example.com/screenshot8.png)
2. **Add Token to GitHub Secrets**: In your repository, go to "Settings" > "Secrets" and add your token as `PERSONAL_ACCESS_TOKEN`.
   ![Add Token to GitHub Secrets](https://example.com/screenshot9.png)

### Step 5: Set Up the Repository

1. **Clone the Repository**: Clone this repository to your local machine.
   ![Clone the Repository](https://example.com/screenshot10.png)
2. **Configure the Environment Variables**: Set up your `.env` file or configure your secrets in GitHub Actions to include `DISCORD_WEBHOOK` and any other necessary tokens.
   ![Configure the Environment Variables](https://example.com/screenshot11.png)

### Step 6: Automate the Workflow with GitHub Actions

1. **Create GitHub Actions**: Use the provided workflow files in the `.github/workflows` directory to automate job listing checks and Discord notifications.
   ![Create GitHub Actions](https://example.com/screenshot12.png)
2. **Customize the Bot**: Modify the scripts as needed to fit your specific requirements.
   ![Customize the Bot](https://example.com/screenshot13.png)

### Step 7: Deploy and Test

1. **Deploy the Bot**: Push your changes to GitHub to trigger the GitHub Actions workflows.
   ![Deploy the Bot](https://example.com/screenshot14.png)
2. **Test the Bot**: Ensure the bot is posting job listings correctly in your specified Discord channel.
   ![Test the Bot](https://example.com/screenshot15.png)
