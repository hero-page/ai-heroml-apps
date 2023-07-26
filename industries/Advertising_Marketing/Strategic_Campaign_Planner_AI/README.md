# Strategic Campaign Planner AI

Strategic Campaign Planner AI allows users to specify variables, harnessing the power of AI to generate a detailed, bespoke strategic plan for a marketing campaign. It defines campaign objectives, identifies target audiences, lays out key messages, chooses marketing channels, decides tactics, sets a timeline, allocates budget, and includes evaluation criteria to measure success. The highlight of this app is its unique, data-driven evaluation criteria. This offers continuous improvement, strategic adaptation and achievement of desired results.

To run this app online: [Strategic Campaign Planner AI Online](https://hero.page/app/strategic-campaign-planner-ai-ai-powered-evaluation-driven-campaign-planning/oSygMmnZ6zT8NWWNfhLk)

To learn more about AI Apps for Marketing Manager use-cases in the Advertising & Marketing industry, read [How to Transform Marketing Strategy with Top AI Workflow Apps](https://hero.page/blog/ai/advertising-and-marketing/how-to-transform-marketing-strategy-with-top-ai-workflow-apps/170718)

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
npx hero run ./strategic_campaign_planner_ai.heroml
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
hero run ./strategic_campaign_planner_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./strategic_campaign_planner_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./strategic_campaign_planner_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./strategic_campaign_planner_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Strategic Campaign Planner AI
```
To create a "Campaign Strategy" for the "Advertising & Marketing" industry for a "Marketing Manager", let's start with the first step: 

1. Generate an executive summary that encapsulates the entire campaign. The summary should include the campaign's key objectives and goals, and it should be written in a concise manner. 

Here's some more context about the Campaign Strategy:
Campaign Overview: {{campaign_overview}}
Campaign Objectives: {{campaign_objectives}}
Target Audience: {{target_audience}}
Key Messages: {{key_messages}}
Marketing Channels: {{marketing_channels}}
Campaign Timeline Budget: {{campaign_timeline_budget}}
Campaign Evaluation: {{campaign_evaluation}}

->>>>

Now that we have an executive summary:

Executive Summary:
{{step_1}}

Let's continue with creating an introduction that explains the broader context of the campaign, considering factors such as market conditions, competitor activities, and customer trends. It should also specify the main objectives of the campaign.

->>>>

We have an executive summary and an introduction for our campaign:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Now, let's proceed with a detailed description of the target audience, focusing on demographic information, behavioral traits, and lifestyle preferences.

->>>>

We have the introduction and an overview of the target audience:

Introduction:
{{step_2}}

Target Audience:
{{step_3}}

Let's proceed with defining the key messages of the campaign that align with your brand identity and value proposition for consistency and cohesion.

->>>>

We have defined our target audience and the key campaign messages:

Target Audience:
{{step_3}}

Key Messages:
{{step_4}}

Next, identify the ideal marketing channels that correspond to the target audience's preferences and behaviors.

->>>>

With details of the target audience, the key messages, and now the marketing channels:

Target Audience:
{{step_3}}

Key Messages:
{{step_4}}

Marketing Channels:
{{step_5}}

Define specific tactics to be used across the chosen marketing channels, including clear actions and motivations behind these decisions.

->>>>

We have the marketing channels and the associated tactics to employ:

Marketing Channels:
{{step_5}}

Tactics:
{{step_6}}

Next, let's discuss the budget, timeline, and the resources required for the campaign execution. Allocation for each component of the campaign should be detailed clearly.

->>>>

The campaign tactics and the timeline, budget, and resource plan is clear:

Tactics:
{{step_6}}

Campaign Budget and Timeline:
{{step_7}}

Establish a strategy for monitoring and evaluating the campaign's success. Earmark the key metrics, KPIs, and a contingency plan for adjustments if required.


```

