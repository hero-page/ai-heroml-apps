# Academic Report AI Creator

Academic Report AI Creator is a ground-breaking app that uses AI to generate customized, intricate academic reports. Users simply specify variables, and the AI compiles well-structured content, featuring abstract, introduction, literature review, methodology, results, discussion and conclusion around any research problem. Delivering analysis of past studies, clear research outlines, unbiased findings, comparisons to previous research, and potential implications, this comprehensive academic report stands in a class of its own. Ideal for the University & Academic industry, this unique tool specializes in complex academic language and concepts.

To run this app online: [Academic Report AI Creator Online](https://hero.page/app/academic-report-ai-creator-ai-powered-academic-report-generator/WdjMmRPrI0f3m6AGtiTw)

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
npx hero run ./academic_report_ai_creator.heroml
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
hero run ./academic_report_ai_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_report_ai_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_report_ai_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_report_ai_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Report AI Creator
```
To generate a "Data Analysis Report" in the "Academic & University" industry for a "Researcher", follow the steps outlined below:

Starting, let's write an informative abstract that provides an overview of the data analysis report, including the research problem, methodologies, major findings, and implications. 

Here's some more context about the Data Analysis Report:
Abstract Overview: {{abstract_overview}}
Research Problem: {{research_problem}}
Literature Review: {{literature_review}}
Methodology: {{methodology}}
Data Findings: {{data_findings}}
Discussion Points: {{discussion_points}}
Conclusion Points: {{conclusion_points}}
Reference List: {{reference_list}}

->>>>

We have begun our Data Analysis Report with:

Abstract Overview:
{{step_1}}

Moving forward, let's develop an introduction that defines the research problem, explains its importance, and states the objectives of the research.

->>>>

We have crafted an Introduction for our Data Analysis Report that builds on the abstract:

Abstract Overview:
{{step_1}}

Introduction:
{{step_2}}

We need to incorporate a literature review section next. This section should summarize previous research studies related to your topic, providing context for our own research and emphasizing the need for our study.

->>>>

We now have an Introduction and a Literature review for our Data Analysis Report:

Introduction:
{{step_2}}

Literature Review:
{{step_3}}

Let's proceed with the methodology section that clearly outlines the procedures used in the research process, including data collection and analysis methods.

->>>>

Our Data Analysis Report now includes an Introduction, Literature review, and Methodology:

Introduction:
{{step_2}}

Literature Review:
{{step_3}}

Methodology:
{{step_4}}

In the results section, we should present the outcomes of our data analysis. Let's generate this section by summarizing the findings without interpretation.

->>>>

Our Data Analysis Report now includes the Results as well:

Methodology:
{{step_4}}

Results:
{{step_5}}

The next section is the Discussion, where we shall interpret the results, compare them with previous studies, and discuss implications for future research.

->>>>

Our Data Analysis Report now includes the Discussion derived from our Results:

Results:
{{step_5}}

Discussion:
{{step_6}}

We should now proceed to the conclusion of the report. Let's put together a conclusion that summarizes the main points of the research, data analysis, the implications of findings, and identifies opportunities for future research.

->>>>

Our Data Analysis Report now includes the Conclusion:

Discussion:
{{step_6}}

Conclusion:
{{step_7}}

To finish off, let's compile a list of references that mention all books, articles, and other resources used in the research.


```

