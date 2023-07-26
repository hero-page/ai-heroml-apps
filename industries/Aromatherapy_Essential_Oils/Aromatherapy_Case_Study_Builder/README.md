# Aromatherapy Case Study Builder

Explore the compelling world of aromatherapy with Aromatherapy Case Study Builder, an AI-powered app that allows users to generate meticulous case studies. Define key variables to guide the AI in crafting rich narratives detailing clients' initial conditions, aromatherapy goals, essential oil selection, and expected therapeutic outcomes. Each study emphasizes real-life scenarios, observable results, and efficacy analysis while preserving client anonymity. By stressing the scientific properties of essentials oils, this app promotes professionalism and credibility in the field.

To run this app online: [Aromatherapy Case Study Builder Online](https://hero.page/app/aromatherapy-case-study-builder-ai-powered-aromatherapy-case-study-creation/h12NPVvD8KBEBy9JtMgK)

To learn more about AI Apps for Aromatherapist use-cases in the Aromatherapy & Essential Oils industry, read [How to Enhance Aromatherapy with AI-Driven Essential Oil Descriptions](https://hero.page/blog/ai/aromatherapy-and-essential-oils/how-to-enhance-aromatherapy-with-ai-driven-essential-oil-descriptions/170729)

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
npx hero run ./aromatherapy_case_study_builder.heroml
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
hero run ./aromatherapy_case_study_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./aromatherapy_case_study_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./aromatherapy_case_study_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./aromatherapy_case_study_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Aromatherapy Case Study Builder
```
Your task is to write a "Client Anonymized Case Study" for the "Aromatherapy & Essential Oils" industry, specifically for an "Aromatherapist". 
To begin, let's create an overview of the client's initial situation, including their presenting condition and goals: {{client_condition}} and {{client_goals}} while ensuring the client's anonymity.

Here's some more context about the Client Anonymized Case Study:
Client Condition: {{client_condition}}
Client Goals: {{client_goals}}
Reason For Aromatherapy: {{reason_for_aromatherapy}}
Essential Oils Selection: {{essential_oils_selection}}
Aromatherapy Sessions: {{aromatherapy_sessions}}
Observed Outcomes: {{observed_outcomes}}
Reflections And Learnings: {{reflections_and_learnings}}
Scientific Evidence: {{scientific_evidence}}

->>>>

The beginning of our case study has been established:

Client's Situation:
{{step_1}}

Next, detail the reason for the client seeking aromatherapy intervention, making sure the client's anonymity is preserved: {{reason_for_aromatherapy}}.

->>>>

Now, we have the beginning of our case study and why the client is seeking aromatherapy:

Client's Situation:
{{step_1}}

Reason for Seeking Aromatherapy:
{{step_2}}

We need to introduce the selection of essential oils and elaborate on the reasons for their choice, giving a description of their expected therapeutic effects: {{essential_oils_selection}}.

->>>>

In our case study, we know the situation, reason for seeking aromatherapy and the essential oil selection:

Client's Situation:
{{step_1}}

Reason for Seeking Aromatherapy:
{{step_2}}

Essential Oils Selection:
{{step_3}}

Next, provide a detailed narrative of the aromatherapy sessions, capturing the progression of the sessions, the reactions, and the effects of the essential oils on the client: {{aromatherapy_sessions}}.

->>>>

In our case study, we have a comprehensive understanding of the aromatherapy sessions, in addition to the earlier points:

Client's Situation:
{{step_1}}

Aromatherapy Sessions:
{{step_4}}

Now, elaborate on the outcomes, noting any changes or improvements seen in the client's condition. Make sure to use both tangible and intangible evidence to back up these observations: {{observed_outcomes}}.

->>>>

In our case study, we've detailed the sessions and the observed outcomes:

Aromatherapy Sessions:
{{step_4}}

Observed Outcomes:
{{step_5}}

We must now write down the reflections and learnings gained from this case study, touching on the effectiveness of the essential oils and process. Always remember to keep the client's identity secured: {{reflections_and_learnings}}.

->>>>

In the case study, along with the detailed sessions and outcomes, we have explored the reflections and learnings:

Aromatherapy Sessions:
{{step_4}}

Reflexions and Learnings:
{{step_6}}

Throughout the case study, let's ensure to emphasize the scientific aspects of essential oils and their therapeutic properties. This will highlight the professional and science-based approach of aromatherapy.


```

