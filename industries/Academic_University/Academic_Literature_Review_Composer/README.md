# Academic Literature Review Composer

The Academic Literature Review Composer, with AI-based literature analysis, permits users to define specific variables. This interactive application uses AI to author custom, high-grade content. The final product offers a complete review of pertinent scholarly literature, entailing an introduction, methodology, synthesized findings, and a critical review. A comprehensive conclusion recaps findings and emphasizes gaps within existing research. The standout feature is the meticulous manner in which it conducts academic literature review, integrating sourcing methodology and linking critical analysis with the research query. The app provides a robust, in-depth understanding of topics, creating uniquely extensive content.

To run this app online: [Academic Literature Review Composer Online](https://hero.page/app/academic-literature-review-composer-comprehensive-ai-based-literature-analysis/NmLPtb6O0xBxTJSiMf9i)

[![Run Academic Literature Review Composer Online](/assets/run.svg)](https://hero.page/app/academic-literature-review-composer-comprehensive-ai-based-literature-analysis/NmLPtb6O0xBxTJSiMf9i)

To learn more about AI Apps for Researcher use-cases in the Academic & University industry, read [How to Enhance Academic Research with AI Tools](https://hero.page/blog/ai/academic-and-university/how-to-enhance-academic-research-with-ai-tools/170699)

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
npx hero run ./academic_literature_review_composer.heroml
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
hero run ./academic_literature_review_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_literature_review_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_literature_review_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_literature_review_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Literature Review Composer
```
Your role is to write a "Literature Review" for the "Academic & University" industry, focusing on a "Researcher". Let's begin with an introduction providing the context for the review while specifying the area of research and the research objectives: {{research_objectives}}.

Here's some more context about the Literature Review:
Research Objectives: {{research_objectives}}
Databases And Search Terms: {{databases_and_search_terms}}
Research Question: {{research_question}}
Research Contribution: {{research_contribution}}
Citation Style: {{citation_style}}

->>>>

We have started our literature review with the following introduction and research objectives:

Introduction and Research Objectives:
{{step_1}}

Now for the methodology section, discuss the ways you have sourced your information. Be sure to specify the databases used and the search terms employed: {{databases_and_search_terms}}.

->>>>

We now have our introduction, research objectives, and our methodology:

Introduction and Research Objectives:
{{step_1}}

Methodology:
{{step_2}}

Let's move towards the synthesis of your findings. Organize the results into themes or sections, ensuring each section relates to the research objectives: {{research_objectives}}.

->>>>

We have completed our introduction, objectives, methodology and now our synthesis of findings: 

Introduction and Research Objectives:
{{step_1}}

Methodology:
{{step_2}}

Synthesis of Findings:
{{step_3}}

Next, draft the interpretation section. Provide a critical analysis of the sampled literature and elaborate how your findings relate to the research question: {{research_question}}.

->>>>

We now have our interpretation of the literature, and how it connects with our research question:
    
Introduction and Research Objectives:
{{step_1}}

Methodology:
{{step_2}}

Synthesis of Findings:
{{step_3}}

Interpretation:
{{step_4}}

In the conclusion section, encapsulate your findings. Point out any gaps in the existing literature, and explain how your research aims to address these gaps: {{research_contribution}}.


```

