# University Fundraising Letter Assistant

University Fundraising Letter Assistant is a practical tool that utilizes AI technology to create personalized, emotionally engaging alumni letters. Users can input specific parameters to generate high-quality content that reminds alumni of their university connection and their crucial role in fostering growth. The AI doesn't merely provide facts but composes letters that demonstrate the impact of past donations, explains the purpose of funding needs and persuasively conveys its benefits, fostering a sense of unity and responsibility towards their alma mater.

To run this app online: [University Fundraising Letter Assistant Online](https://hero.page/app/university-fundraising-letter-assistant-personalized-alumni-fundraising-letters/M3Pz9UWZIHvCYiF7iLtm)

[![Run University Fundraising Letter Assistant Online](/assets/run.svg)](https://hero.page/app/university-fundraising-letter-assistant-personalized-alumni-fundraising-letters/M3Pz9UWZIHvCYiF7iLtm)

To learn more about AI Apps for Alumni Relations Officer use-cases in the Academic & University industry, read [How to Elevate Alumni Outreach with AI-powered Newsletter, Fundraising and Event Invites](https://hero.page/blog/ai/academic-and-university/how-to-elevate-alumni-outreach-with-ai-powered-newsletter-fundraising-and-event-invites/170710)

### What is HeroML?
HeroML is an AI Prompt Chain/Workflow interpreter for Apps built on https://hero.page 

To see other apps, visit the [Hero Apps](https://hero.page/apps) page or explore [AI Apps for all industries](https://hero.page/blog) in the blog section

For more documentation, visit [Hero docs, and learn about AI App Workflows](https://hero.page/tutorials/introduction-to-heroml)

Download [VSCode Syntax Highlighter Ext. here](https://marketplace.visualstudio.com/items?itemName=hero-page.heroml)

## Run with HeroCLI (Requires OpenAI Token)

#### Installation

To install the HeroML CLI tool, you need to have Node.js and npm (comes with Node.js) installed on your machine. If you don't have these, please install them first. 

Then, run the following command in your terminal:

```bash
npm install -g heroml
```

This will install the HeroML CLI tool globally on your system, allowing you to use the `hero` command from any directory.

If you don't want to install it globally, you can run:

```bash
npm install heroml
```

and use it like:

```bash
npx hero run ./university_fundraising_letter_assistant.heroml
```

We'll be using `hero run ...` in this tutorial for simplicity.

#### Configuration

Before using the HeroML CLI tool, you need to configure your OpenAI API key. 

Create a `heroconfig.json` file in your home directory with the following content:

```json
{
  "openaiApiKey": "your-openai-api-key"
}
```

Replace `"your-openai-api-key"` with your actual OpenAI API key.

#### Usage

To run a HeroML script, use the `run` command followed by the path to your script:

```bash
hero run ./university_fundraising_letter_assistant.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./university_fundraising_letter_assistant.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./university_fundraising_letter_assistant.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./university_fundraising_letter_assistant.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for University Fundraising Letter Assistant
```
Your task is to write a "Fundraising Letter" for the "Academic & University" industry, specifically for an "Alumni Relations Officer". 
Let's start by creating a warm greeting to address the audience.

Here's some more context about the Fundraising Letter:
Salutation: {{salutation}}
University Achievements: {{university_achievements}}
Funding Purpose: {{funding_purpose}}
Benefits Of Funding: {{benefits_of_funding}}
Importance Of Alumni Support: {{importance_of_alumni_support}}
Impact Of Previous Donations: {{impact_of_previous_donations}}
Sign Off: {{sign_off}}

->>>>

We now have a warm greeting to use in the letter:

Salutation:
{{step_1}}

Now, write an introduction that reminds the recipient of their connection to the University by sharing some key achievements or notable events from the University.

->>>>

We have a salutation and an introduction that establishes the recipient's connection to the University:

Salutation:
{{step_1}}

Introduction:
{{step_2}}

Next, articulate the purpose of the letter by introducing the requirement to raise funds for a particular need, such as a new academic program or construction project.

->>>>

The introduction to our fundraiser letter is:

Introduction:
{{step_2}}

Here is the purpose of our fundraising:

Purpose:
{{step_3}}

After that, provide future benefits that the funding can bring, within the four W’s structure - who will benefit, what will change, when will results show, and why this is crucial for growth.

->>>>

We have articulated the purpose of our fundraising:

Purpose:
{{step_3}}

Here are the potential benefits of the funds:

Benefits:
{{step_4}}

Now, provide a detailed explanation of the donation process and the different giving options available such as online, bank transfer, and check, to personalize it for different donor preferences.

->>>>

We've explained the potential beneficiaries of our fund and the changes it would bring:

Benefits:
{{step_4}}

Here's an explanation of the donation process and the different giving options available:

Donation Process and Options:
{{step_5}}

Follow this by highlighting the importance of alumni support.

->>>>

Our explanation of the donation process includes the following:

Donation Process and Options:
{{step_5}}

Here is why alumni support is crucial for us:

Importance of Alumni Support:
{{step_6}}

Next, share personal stories of how previous alumni donations have made a difference to reinforce the positive impact of giving.

->>>>

We have emphasized the necessity of alumni support:

Importance of Alumni Support:
{{step_6}}

Here are the impacts of the previous alumni donations:

Impact of Previous Donations:
{{step_7}}

Now, let's conclude the letter by thanking the recipient for their continued support and loyalty towards the University.

->>>>

We've shown the impact of alumni donations:

Impact of Previous Donations:
{{step_7}}

Here's a thank-you note to express our gratitude:

Thank-you note:
{{step_8}}

Finally, show your appreciation by writing a personalized sign-off that also exudes the spirit of the University.


```

