# Graduate Dissertation AI Composer

Graduate Dissertation AI Composer is an advanced application that uses AI to create top-notch academic dissertations tailored for graduate students. Packed with features that allow users to specify unique variables in writing prompts, it produces a comprehensive study containing an abstract, introduction, literature review, methodology, research findings, study implications, and conclusion. Notably, it expertly integrates chosen university's citation style and provides clear research outlines, insightful findings, and potential areas for future study. Its precise attention to academic standards and in-depth detail set it apart.

To run this app online: [Graduate Dissertation AI Composer Online](https://hero.page/app/graduate-dissertation-ai-composer-ai-powered-academic-dissertation-crafting/ME4iKAY5lVNRIV6YTjrv)

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
npx hero run ./graduate_dissertation_ai_composer.heroml
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
hero run ./graduate_dissertation_ai_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./graduate_dissertation_ai_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./graduate_dissertation_ai_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./graduate_dissertation_ai_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Graduate Dissertation AI Composer
```
Your task is to draft a "Dissertation" for the "Academic & University" industry, for a "Graduate Student". 
The first step is to create an abstract that gives an overview of the study: {{study_overview}}.

Here's some more context about the Dissertation:
Study Overview: {{study_overview}}
Study Context: {{study_context}}
Related Literature: {{related_literature}}
Research Methodology: {{research_methodology}}
Research Findings: {{research_findings}}
Study Implications: {{study_implications}}
Study Conclusion: {{study_conclusion}}

->>>>

In our dissertation, we have our abstract:

Abstract:
{{step_1}}

Next, let's write an introduction that provides context to your study: {{study_context}}, it should include your research question/problem statement and the objectives.

->>>>

Our dissertation now has an abstract and an introduction:

Abstract:
{{step_1}}

Introduction:
{{step_2}}

The next requirement is to develop a literature review section that explores previous work related to the subject: {{related_literature}}, it should help justify why your study is unique and necessary.

->>>>

We have in our dissertation an abstract, introduction, and a literature review:

Abstract:
{{step_1}}

Introduction:
{{step_2}}

Literature Review:
{{step_3}}

Now, let's detail your methodology, this should include your research design, data collection methods, and analysis approach: {{research_methodology}}.

->>>>

In our dissertation, we have an abstract, introduction, literature review, and methodology:

Abstract:
{{step_1}}

Introduction:
{{step_2}}

Literature Review:
{{step_3}}

Methodology:
{{step_4}}

Next, present your research findings or result. Discuss the data you gathered: {{research_findings}}. Then, interpret these results in the context of your research question and related literature.

->>>>

We've written an abstract, introduction, literature review, methodology, and research findings:

Abstract:
{{step_1}}

Introduction:
{{step_2}}

Literature Review:
{{step_3}}

Methodology:
{{step_4}}

Research Findings:
{{step_5}}

Now, discuss your study implications, which includes the impact and significance of your research on existing literature and practical implications: {{study_implications}}.

->>>>

Our complete items in the dissertation now include an abstract, introduction, literature review, methodology, research findings, and study implications:

Abstract:
{{step_1}}

Introduction:
{{step_2}}

Literature Review:
{{step_3}}

Methodology:
{{step_4}}

Research Findings:
{{step_5}}

Study Implications:
{{step_6}}

Next, let's draw a conclusion that restates your research problem, summarizes your findings, and gives suggestions for further studies: {{study_conclusion}}.


```

