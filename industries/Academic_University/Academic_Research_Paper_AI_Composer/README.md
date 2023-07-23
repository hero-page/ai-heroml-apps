# Academic Research Paper AI Composer

Explore the future of academic writing with the Academic Research Paper AI Composer. This smart app lets you specify variables in prompts, empowering AI to craft custom, high-quality academic content. It’s designed to produce comprehensive research papers for academia and universities. Expect an abstract, clear problem statement, literature review, thorough methodology, results analysis, informed discussion, and neatly wrapped-up conclusion. It seamlessly integrates industry-specific lingo, acknowledges research limitations, while adhering strictly to academic writing structuring for logical flow & readability. This app's uniqueness lies in generating exhaustive, industry-specific research papers.

To run this app online: [Academic Research Paper AI Composer Online](https://hero.page/app/academic-research-paper-ai-composer-ai-powered-comprehensive-academic-author/L1yrKmPBPPsRiI8vjroO)

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
npx hero run ./academic_research_paper_ai_composer.heroml
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
hero run ./academic_research_paper_ai_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_research_paper_ai_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_research_paper_ai_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_research_paper_ai_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Research Paper AI Composer
```
Your task is to write a Research Paper for the Academic & University industry, specifically designed for a Researcher. 
Let's start by writing an abstract that provides a summary of the entire research: {{research_summary}}.

Here's some more context about the Research Paper:
Research Summary: {{research_summary}}
Research Context: {{research_context}}
Previous Works: {{previous_works}}
Research Design: {{research_design}}
Research Results: {{research_results}}
Findings Interpretation: {{findings_interpretation}}
Research Conclusion: {{research_conclusion}}
Cited Sources: {{cited_sources}}

->>>>

Now, we have the abstract for our research paper:

Abstract:
{{step_1}}

Next, let's write an introduction that provides context to the research topic {{research_context}}, including a clear problem statement and the relevance of the problem.

->>>>

At this point, we have an abstract and introduction for our research paper:

Abstract:
{{step_1}}

Introduction:
{{step_2}}

Now, we should proceed to the literature review section that synthesizes and critiques previous works relating to the research topic {{previous_works}}.

->>>>

We now have an abstract, an introduction, and a literature review for our research paper:

Abstract:
{{step_1}}

Introduction:
{{step_2}}

Literature review:
{{step_3}}

Next, let's write the methodology section that presents the design of the study or experiment: {{research_design}}.

->>>>

We've completed the methodology section, and so far our research paper has the following sections:

Abstract:
{{step_1}}

Introduction:
{{step_2}}

Literature Review:
{{step_3}}

Methodology:
{{step_4}}

Now, we need to discuss and analyze the results or findings from your study or experiment in a results section: {{research_results}}.

->>>>

At this point, our research paper with the abstract, introduction, literature review, methodology, and results sections:

Abstract:
{{step_1}}

Introduction:
{{step_2}}

Literature Review:
{{step_3}}

Methodology:
{{step_4}}

Results:
{{step_5}}

Next, provide an interpretation of your findings in a discussion section, relating them to the existing knowledge in the field: {{findings_interpretation}}.

->>>>

Our research has the following parts:

Abstract:
{{step_1}}

Introduction:
{{step_2}}

Literature Review:
{{step_3}}

Methodology:
{{step_4}}

Results:
{{step_5}}

Discussion:
{{step_6}}

Now, it's time to conclude the research paper with a summary of the whole research, emphasizing the key findings and their implications in the field: {{research_conclusion}}.


```

