# Academic Essay Analysis & Execution AI

Academic Essay Analysis & Execution AI is a sophisticated tool designed to craft adept, thesis-driven essays. Using cutting-edge AI technology, users specify variables which the app translates into a detailed, customized essay. It encapsulates a clear thesis statement, analysis, and evidence in structured sections, demonstrating critical thinking, reflection, and academic language use. Its unique feature lies in generating comprehensive academic content, incorporating discipline-specific terminology and presenting a thorough argument with a structured conclusion. It fosters precision with proofreading and a correctly formatted reference list.

To run this app online: [Academic Essay Analysis & Execution AI Online](https://hero.page/app/academic-essay-analysis-and-execution-ai-smart-thesis-driven-essay-generator/lZjO5ysW9h9suT8CNhBg)

[![Run Academic Essay Analysis & Execution AI Online](/assets/run.svg)](https://hero.page/app/academic-essay-analysis-and-execution-ai-smart-thesis-driven-essay-generator/lZjO5ysW9h9suT8CNhBg)

To learn more about AI Apps for Undergraduate Student use-cases in the Academic & University industry, read [How to Ace University Writing with AI Academic Assistance](https://hero.page/blog/ai/academic-and-university/how-to-ace-university-writing-with-ai-academic-assistance/170701)

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
npx hero run ./academic_essay_analysis_and_execution_ai.heroml
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
hero run ./academic_essay_analysis_and_execution_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_essay_analysis_and_execution_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_essay_analysis_and_execution_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_essay_analysis_and_execution_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Essay Analysis & Execution AI
```
Your task is to write an "Essay" for the "Academic & University" industry, specifically for an "Undergraduate Student". 
Let's begin with an engaging introduction that explains the topic or argument {{essay_topic}}. Be sure to include a thought-provoking title or question, a jargon-free definition of the topic, and a concise thesis statement.

Here's some more context about the Essay:
Essay Topic: {{essay_topic}}
Primary Points: {{primary_points}}
Supporting Evidence: {{supporting_evidence}}

->>>>

We are creating an academic essay on the domain of {{essay_topic}}. We have an engaging introduction for our essay:

Introduction:
{{step_1}}

Next, let's divide the essay into coherent sections. Each section should focus on one out of the {{primary_points}}, which could be fact-based arguments, an analysis of specific aspects of the topic, or critique and commentary on existing literature.

->>>>

We have divided the essay into structured sections, each focusing on a primary point. Our essay now looks as follows:

Introduction:
{{step_1}}

Primary Points:
{{step_2}}

Moving on, let's embellish each section with relevant supporting evidence {{supporting_evidence}}. This can include observations, anecdotes, research data, references to academic materials or real-world examples related to the topic.

->>>>

For each of our primary points, we have included supporting evidence. Our essay's body contains:

Primary Points with Evidence:
{{step_3}}

Now, incorporate critical analysis and reflection throughout the essay. Examine and explain the implications, significance, and impact of your evidence, and how it reinforces your supporting point and overall thesis.

->>>>

With detailed critical analysis, our essay consists of:

Evidence with Critical Analysis:
{{step_4}}

For the language and style, use academic language consistently, incorporating industry-specific insights and terminology that demonstrate your understanding of the {{essay_topic}} and its relevance to your field of study.

->>>>

With precise academic language, our essay is composed as follows:

Essay with Academic Language:
{{step_5}}

Now, let's summarize, interpret, and synthesize your arguments. Restate your thesis in light of the evidence you have presented, and include your final conclusions or recommendations regarding the {{essay_topic}}.

->>>>

We have a conclusion for our essay, summarizing, interpreting, and synthesizing our arguments:

Essay with Conclusion:
{{step_6}}

Next, append a properly formatted reference list to credit all sources you have referenced in the essay according to the referencing style that is standard in your university.


```

