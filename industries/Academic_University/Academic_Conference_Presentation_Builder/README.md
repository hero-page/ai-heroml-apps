# Academic Conference Presentation Builder

The Academic Conference Presentation Builder transforms your research into detailed presentations. Craft engaging slides highlighting your study's motivation, objectives, and methodologies. Leverage advanced AI to generate informed findings, implications, and impactful summaries. Communicate your contributions effectively to the academic community using appropriate language and citations. The app will also help you place your research in the context of larger industry trends. The unique aspect? Your research isn't just outlined, but showcased in comprehensive detail, demonstrating a deep understanding of your academic field.

To run this app online: [Academic Conference Presentation Builder Online](https://hero.page/app/academic-conference-presentation-builder-transforming-research-into-presentations/v0qLY1YXRc5L5MiJMbF8)

[![Run Academic Conference Presentation Builder Online](/assets/run.svg)](https://hero.page/app/academic-conference-presentation-builder-transforming-research-into-presentations/v0qLY1YXRc5L5MiJMbF8)

To learn more about AI Apps for Graduate Student use-cases in the Academic & University industry, read [How to Elevate University Research with AI Assistance](https://hero.page/blog/ai/academic-and-university/how-to-elevate-university-research-with-ai-assistance/170700)

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
npx hero run ./academic_conference_presentation_builder.heroml
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
hero run ./academic_conference_presentation_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_conference_presentation_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_conference_presentation_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_conference_presentation_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Conference Presentation Builder
```
Your task is to write a "Conference Presentation" for the "Academic & University" industry, specifically for a "Graduate Student". Let's start by creating an attention-grabbing introduction that sets the context and speaks about the motivation behind the research: {{research_motivation}}.

Here's some more context about the Conference Presentation:
Research Motivation: {{research_motivation}}
Research Question: {{research_question}}
Research Methods: {{research_methods}}
Major Findings: {{major_findings}}

->>>>

We now have an introduction to our presentation:

Introduction:
{{step_1}}

Following the introduction, let's form a research question, hypothesis, or objective, hereafter referred to as {{research_question}}.

->>>>

We now have the introduction and the research question for our presentation:

Introduction:
{{step_1}}

Research Question:
{{step_2}}

Next, we need to explain the methodologies i.e., {{research_methods}}, that were used during the process of this research.

->>>>

We now have the introduction, research question, and methodology for our presentation:

Introduction:
{{step_1}}

Research Question:
{{step_2}}

Methodologies:
{{step_3}}

Following this, let's present the major findings or key arguments, also called as {{major_findings}}, that this research has yielded.

->>>>

Up to now, we have prepared the introduction, research question, methodology, and major findings for our presentation:

Introduction:
{{step_1}}

Research Question:
{{step_2}}

Methodologies:
{{step_3}}

Major Findings:
{{step_4}}

Now, we need to discuss the implications of these findings in relation to existing theories and previous research. We also want to present new questions that these findings raise for future research.

->>>>

We now have a discussion on the existing theories, previous research and new questions for future research in relation to our major findings:

Introduction:
{{step_1}}

Research Question:
{{step_2}}

Major Findings:
{{step_4}}

Discussion of Findings:
{{step_5}}

To wrap this all up, let's produce a summary for the presentation. This should include reiteration of the research question and the impact of the findings on the larger conversation within the field.


```

