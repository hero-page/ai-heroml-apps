# Aromatherapy Guide & Case Study Creator

Enhancing your aromatherapy knowledge with Aromatherapy Guide and Case Study Creator. This AI-powered app lets you specify variables in prompts to generate custom, high-quality guides on aromatherapy and essential oils. Content includes details on purpose, history, principles, oil profiles, blending guidelines, safety measures and usage for conditions. Uniquely, the app offers illustrative case studies that provide real-life application examples for novices and experts alike. Dive into the world of aromatherapy with the most comprehensive, practical resource at your fingertips.

To run this app online: [Aromatherapy Guide & Case Study Creator Online](https://hero.page/app/aromatherapy-guide-and-case-study-creator-case-studies-for-aromatherapy-mastery/53CnbKQCGMBNfpffVhIP)

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
npx hero run ./aromatherapy_guide_and_case_study_creator.heroml
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
hero run ./aromatherapy_guide_and_case_study_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./aromatherapy_guide_and_case_study_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./aromatherapy_guide_and_case_study_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./aromatherapy_guide_and_case_study_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Aromatherapy Guide & Case Study Creator
```
Your task is to write a "Therapy Guide" for the "Aromatherapy & Essential Oils" industry, specifically for an "Aromatherapist". 

Begin by writing an introduction that explains the purpose of this therapy guide. Make sure it's clear and concise, and focus on discussing the benefits of "Aromatherapy & Essential oils" in relation to the intended purpose.

Here's some more context about the Therapy Guide:
Purpose: {{purpose}}
Extraction Methods And Uses: {{extraction_methods_and_uses}}
Essential Oil Profile: {{essential_oil_profile}}
Blending And Safety Guidelines: {{blending_and_safety_guidelines}}
Condition Based Essential Oils: {{condition_based_essential_oils}}
Case Studies: {{case_studies}}
Guide Value: {{guide_value}}

->>>>

Now we have a clear introduction to our Therapy Guide:

Introduction:
{{step_1}}

Moving on, write a section that introduces the history and fundamental principles of "Aromatherapy & Essential Oils". Explain the different ways essential oils are extracted and their varied uses in therapy.

->>>>

We have an introduction and an overview of the history and principles of Aromatherapy:

Introduction:
{{step_1}}

History and Principles:
{{step_2}}

The next step is to compile a comprehensive list of essential oils. Detail the specific benefits and therapeutic uses of each, discussing the benefits, contraindications, and methods of use where relevant.

->>>>

We have detailed the history and principles, and created a comprehensive list of essential oils:

History and Principles:
{{step_2}}

Essential Oils List:
{{step_3}}

Now, draft guidelines on the correct methods of blending essential oils and the safety precautions to take.

->>>>

We have a comprehensive list of essential oils and a crafted set of guidelines for blending and safety:

Essential Oils List:
{{step_3}}

Blending and Safety Guidelines:
{{step_4}}

Let's navigate towards introducing the concept of "Aromatherapy & Essential oils" for different conditions. Categorize these based on the conditions the aromatherapist will be treating.

->>>>

We have our guidelines for blending and safety, and a categorized list of essential oils based on conditions:

Blending and Safety Guidelines:
{{step_4}}

Condition-Based Essential Oils:
{{step_5}}

Now, write up a series of case studies that illustrate the application of aromatherapy. Discuss each case's initial condition, the essential oils used, and the outcome of the therapy.

->>>>

We have a list of condition-based essential oils and a series of illustrative case studies:

Condition-Based Essential Oils:
{{step_5}}

Case Studies:
{{step_6}}

Follow this up by concluding the guide with an appendix section. Include a glossary of relevant terms, useful websites or books for further reading, and an index for easy navigation.

->>>>

Now we have a set of illustrative case studies and a comprehensive appendix for our guide:

Case Studies:
{{step_6}}

Appendix:
{{step_7}}

Finally, summarize the Therapy Guide with a conclusion which reiterates the value of the guide and how it contributes to improving the aromatherapist's work.


```

