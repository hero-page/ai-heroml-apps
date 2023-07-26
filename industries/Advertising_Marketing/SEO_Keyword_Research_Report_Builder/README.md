# SEO Keyword Research Report Builder

Turn your SEO strategy into a powerhouse with the SEO Keyword Research Report Builder. Unlock a detailed Keyword Research Report, tailored to your business's needs. Harness the power of AI to discover high-quality content, industry specifics, target audience, keyword analytics, competitor analysis, and an actionable optimization plan. Get the perfect balance of short and long tail keywords, identify opportunities, and tackle challenges effectively. Plus, get insights into the process and tools used for keyword research. Customize your SEO game for the Advertising and Marketing sector like never before.

To run this app online: [SEO Keyword Research Report Builder Online](https://hero.page/app/seo-keyword-research-report-builder-tailored-seo-keyword-strategy-builder/xlWTco9Bfq3ZQ9QS9rOL)

To learn more about AI Apps for SEO Specialist use-cases in the Advertising & Marketing industry, read [How to Generate SEO Keyword Reports and Optimized Articles with AI](https://hero.page/blog/ai/advertising-and-marketing/how-to-generate-seo-keyword-reports-and-optimized-articles-with-ai/170717)

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
npx hero run ./seo_keyword_research_report_builder.heroml
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
hero run ./seo_keyword_research_report_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./seo_keyword_research_report_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./seo_keyword_research_report_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./seo_keyword_research_report_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for SEO Keyword Research Report Builder
```
Your task is to create a "Keyword Research Report" for the "Advertising & Marketing" industry, specifically for a "SEO Specialist". 

Let's start by generating an executive summary that provides an overview of the keyword research performed: {{summary_keyword_research}}. This should highlight the objective of the report and the key findings.

Here's some more context about the Keyword Research Report:
Summary Keyword Research: {{summary_keyword_research}}
Business Context: {{business_context}}
Tools Used: {{tools_used}}
Target Audience: {{target_audience}}
Short Tail Keywords: {{short_tail_keywords}}
Long Tail Keywords: {{long_tail_keywords}}
Competitor Keywords: {{competitor_keywords}}
Opportunity Keywords: {{opportunity_keywords}}
Challenging Keywords: {{challenging_keywords}}
Chosen Keywords Plan: {{chosen_keywords_plan}}

->>>>

We have an executive summary for our keyword research report:

Executive Summary:
{{step_1}}

Moving on, let's create an introduction. This should explain the business context {{business_context}}, why the keyword research was performed, its significance to SEO, and how it ties into the overarching marketing objective.

->>>>

For our keyword research report, we have an executive summary and an introduction:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Next, provide a detailed account of the keyword research process that was undertaken. This should cover the tools or software used {{tools_used}}, data sources, and the time period the research was conducted over.

->>>>

Our keyword research report has a clear executive summary, introduction, and a detailed report on the research process:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Keyword Research Process:
{{step_3}}

Now, describe the target audience specific to the industry and how this influenced your keyword selection: {{target_audience}}.

->>>>

For our keyword research report, we have an executive summary, introduction, keyword research process, and a detailed description of the target audience:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Keyword Research Process:
{{step_3}}

Target Audience:
{{step_4}}

Next, write a detailed analysis section reporting on the specific keywords. These should be segmented into: 
- Short Tail Keywords: Discuss the high traffic, broad {{short_tail_keywords}} that were found. 
- Long Tail Keywords: Highlight the specific, lower traffic {{long_tail_keywords}} that were identified. 
- Competitor Analysis: Reveal the {{competitor_keywords}} your competitors rank for but you don't.

->>>>

Now, we have an analysis of the keywords for the keyword research report:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Keyword Research Process:
{{step_3}}

Target Audience:
{{step_4}}

Keyword Analysis:
{{step_5}}

Next, outline potential opportunities for ranking based on the keyword analysis performed. Which keywords {{opportunity_keywords}} could the business potentially take advantage of?

->>>>

For our keyword research report, we have an executive summary, introduction, keyword research process, a detailed description of the target audience, keyword analysis, and a discussion of potential opportunities:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Keyword Research Process:
{{step_3}}

Target Audience:
{{step_4}}

Keyword Analysis:
{{step_5}}

Opportunities:
{{step_6}}

Now, pen down a section discussing possible challenges in trying to rank for certain popular keywords {{challenging_keywords}} within the industry.

->>>>

Our keyword research report has most of the sections, including a section discussing challenges:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Keyword Research Process:
{{step_3}}

Target Audience:
{{step_4}}

Keyword Analysis:
{{step_5}}

Opportunities:
{{step_6}}

Challenges:
{{step_7}}

Next, generate a conclusion that reiterates the key findings, opportunities, challenges, and assesses how these fit into the wider SEO campaign of the company.


```

