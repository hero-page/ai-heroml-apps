# Cannabis Cultivation Guide Creator

The Cannabis Cultivation Guide Creator app offers a personalized growing experience for cannabis cultivators. Pose your queries and AI-powered algorithms will churn out high-quality, tailored instructions on cannabis farming. Learn about soil, climate and growth conditions, detailed growth processes, disease prevention measures, and yield maximization tips. This app is your solution to a comprehensive guide uniquely designed for cultivators in the Cannabis Industry, emphasizing sustainability practices.

To run this app online: [Cannabis Cultivation Guide Creator Online](https://hero.page/app/cannabis-cultivation-guide-creator-customized-cannabis-cultivation-guide/G7CvmoXSNxWlfW3Uqcg2)

[![Run Cannabis Cultivation Guide Creator Online](/assets/run.svg)](https://hero.page/app/cannabis-cultivation-guide-creator-customized-cannabis-cultivation-guide/G7CvmoXSNxWlfW3Uqcg2)

To learn more about AI Apps for Cultivator use-cases in the Cannabis Industry industry, read [How to Elevate Cannabis Cultivation with AI Guide Apps](https://hero.page/blog/ai/cannabis-industry/how-to-elevate-cannabis-cultivation-with-ai-guide-apps/170769)

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
npx hero run ./cannabis_cultivation_guide_creator.heroml
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
hero run ./cannabis_cultivation_guide_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./cannabis_cultivation_guide_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./cannabis_cultivation_guide_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./cannabis_cultivation_guide_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Cannabis Cultivation Guide Creator
```
Let's write a "Grow Guide" for the "Cannabis Industry" industry, specifically for a "Cultivator". 
First, let's write an introduction that explains the purpose and benefits of the guide: {{guide_purpose}}.

Here's some more context about the Grow Guide:
Guide Purpose: {{guide_purpose}}
Fundamental Necessities: {{fundamental_necessities}}
Cultivation Process: {{cultivation_process}}
Common Issues: {{common_issues}}
Growth Stages: {{growth_stages}}
Best Practices: {{best_practices}}

->>>>

Now we have an introduction for our "Grow Guide":

Introduction:
{{step_1}}

Next, discuss the fundamental necessities for cannabis growth including soil type, climate, and ideal conditions: {{fundamental_necessities}}.

->>>>

We have an introduction and discussion of fundamental necessities for the guide:

Introduction:
{{step_1}}

Fundamental Necessities:

{{step_2}}

Let's now provide details on the cultivation process from sowing seeds or clones, all the way to the curing and storage of harvested cannabis: {{cultivation_process}}.

->>>>

So far, in our guide we have an introduction, discussed fundamental necessities, and detailed the cultivation process:

Introduction:
{{step_1}}

Fundamental Necessities:
{{step_2}}

Cultivation Process:
{{step_3}}

Next, let's infuse a section around common parasite and disease issues that cultivators might come across and measures for prevention or control: {{common_issues}}

->>>>

In our guide we have discussed the cultivation process and have also detailed common issues faced by cultivators and their solutions:

Cultivation Process:
{{step_3}}

Common Issues and Solutions:
{{step_4}}

Now, it's essential to provide a detailed guide on the various stages of cannabis plant growth, explaining what to expect and how to maximize yield for each stage: {{growth_stages}}.


```

