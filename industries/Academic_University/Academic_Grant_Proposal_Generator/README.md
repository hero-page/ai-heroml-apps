# Academic Grant Proposal Generator

Discover the power of AI with the Academic Grant Proposal Generator: an AI-Powered Academic Grant Writer. Tailor your prompts to generate customised, professional and compelling letters of inquiry for academic grants. From outlining your project, explaining its purpose, summarizing its objectives and methodology, to detailing funding usage, the app crafts a narratively rich and persuasive proposal. Designed specifically for academia, it embodies the formal, professional tone required while highlighting your unique needs and solutions.

To run this app online: [Academic Grant Proposal Generator Online](https://hero.page/app/academic-grant-proposal-generator-ai-powered-academic-grant-writer/S9hUwpqgAb7gQbfsGOAe)

To learn more about AI Apps for Grant Writer use-cases in the Academic & University industry, read [How to Streamline Grant Writing in Academia with AI Apps](https://hero.page/blog/academic-and-university/grant-writer/how-to-streamline-grant-writing-in-academia-with-ai-apps/170704)

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
npx hero run ./academic_grant_proposal_generator.heroml
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
hero run ./academic_grant_proposal_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_grant_proposal_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_grant_proposal_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_grant_proposal_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Grant Proposal Generator
```
Your task is to write a "Letter of Inquiry" for the "Academic & University" industry, aimed toward a "Grant Writer". Let's start by drafting an introduction that explains the purpose of the letter, your interest in the funding opportunity: {{funding_interest}}, and introduces the organization you are representing: {{your_organization}}.

Here's some more context about the Letter of Inquiry:
Funding Interest: {{funding_interest}}
Your Organization: {{your_organization}}
Project Needs: {{project_needs}}
Project Solution: {{project_solution}}
Grant Usage: {{grant_usage}}
Your Name And Title: {{your_name_and_title}}

->>>>

With the introduction for the letter of inquiry drafted:

Introduction:
{{step_1}}

Let's now write the second paragraph. Talk about the need or problem that your project or research aims to address: {{project_needs}}. Make sure to back up this section with substantial data or evidence to strengthen your case.

->>>>

In our "Letter of Inquiry", this is our introduction and the highlighted problem or need:

Introduction:
{{step_1}}

Problem/Need:
{{step_2}}

Now, describe specifically how your project or research will provide a solution to the identified problem or need: {{project_solution}}. This description should include a brief summary of your project's objectives, methodology, and expected outcomes.

->>>>

For our "Letter of Inquiry", we have the identified problem/need and our proposed solution:

Problem/Need:
{{step_2}}

Proposed Solution:
{{step_3}}

In the next paragraph, detail how the grant will be used if awarded: {{grant_usage}}. This information should include a rough estimate of the project budget and specify how the funds will support the achievement of the project's objectives.

->>>>

In our "Letter of Inquiry" we now have the proposed solution and details of grant usage:

Proposed Solution:
{{step_3}}

Grant Usage:
{{step_4}}

Now, conclude the letter with a call to action, encouraging the grantor to consider your proposal. Please express your readiness to provide further information as needed.

->>>>

With the call to action, our "Letter of Inquiry" now includes the grant usage and a conclusion urging the grantor's consideration:

Grant Usage:
{{step_4}}

Conclusion/Call to Action:
{{step_5}}

Always end the letter by appreciating the grantor's time and consideration. This should be followed by a formal closing ('Yours sincerely'), and your full name and title: {{your_name_and_title}}.


```

