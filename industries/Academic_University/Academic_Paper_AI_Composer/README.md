# Academic Paper AI Composer

Create and explore scholarly papers with Academic Paper AI Composer. Craft comprehensive sections such as the abstract, introduction, methodology, results, and conclusion using AI technology. Specify your research question, engage peers, and inspire discussions. The uniquely complex and detailed output resonates professionalism and knowledge, reflecting the complex nature of academic papers.

To run this app online: [Academic Paper AI Composer Online](https://hero.page/app/academic-paper-ai-composer-ai-crafted-comprehensive-research-papers/LSHw5g9ntEXY2f9fyqxJ)

To learn more about AI Apps for Professor use-cases in the Academic & University industry, read [How to Automate Academic Writing with AI Tools](https://hero.page/blog/academic-and-university/professor/how-to-automate-academic-writing-with-ai-tools/170698)

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
npx hero run ./academic_paper_ai_composer.heroml
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
hero run ./academic_paper_ai_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_paper_ai_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_paper_ai_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_paper_ai_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Paper AI Composer
```

To create an "Academic Paper" in the "Academic & University" industry for a "Professor", follow these steps:

Start the paper with an "Abstract" that summarizes the research topic and the key findings: {{research_topic}}.

Here's some more context about the Academic Paper:
Research Topic: {{research_topic}}
Research Question: {{research_question}}
Research Methods: {{research_methods}}

->>>>

Now we have an abstract for our academic paper:

Abstract:
{{step_1}}

Next, let's proceed with an "Introduction" that presents the research question or hypothesis: {{research_question}} and outlines the significance of the study in the academic field.

->>>>

Now, we have the introduction for our academic paper:

Introduction:
{{step_2}}

Moving on, create a comprehensive "Literature Review" to discuss existing research related to {{research_topic}} and identify the gaps that your paper intends to fill.

->>>>

Now, we have an established literature review for our academic paper:

Literature Review:
{{step_3}}

Let's now detail the "Methodology" section. Here, describe the research methods and materials used: {{research_methods}}, and provide a justification for their choice.

->>>>

We are progressing with our academic paper. We now have the methodology section:

Methodology:
{{step_4}}

Our next step involves presenting your findings in the "Results" section, which should answer or address the {{research_question}}.

->>>>

Up to this point, we have detailed results for our academic paper:

Results:
{{step_5}}

Let's now turn our focus towards the "Discussion" section and analyze these results. Ensure you link the outcomes back to the {{research_question}} and the broader academic context. Also, clarify the implications of your findings for your field.

->>>>

Our academic paper now has a detailed discussion:

Discussion:
{{step_6}}

Next, draft the "Conclusion" section summarizing the research, reaffirming your findings and their significance to the {{research_topic}}, and suggesting future research directions.

->>>>

Now, we have a conclusion for our academic paper:

Conclusion:
{{step_7}}

Our next step is to compile a "References" list, acknowledging all the sources cited in your paper, aligning with the academic citation style relevant to your field.

->>>>

So far, we have a comprehensive reference list for our academic paper:

References:
{{step_8}}

If applicable, let's add an "Appendices" section for any supplementary information or data, without overloading the main text.

->>>>

For our academic paper, we now have the appendices if necessary:

Appendices:
{{step_9}}

Next, incorporate key phrases and jargon specific to the domain of the {{research_topic}}, this will help to increase both its searchability and credibility.


```

