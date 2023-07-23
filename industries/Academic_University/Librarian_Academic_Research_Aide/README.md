# Librarian Academic Research Aide

The Librarian Academic Research Aide app leverages AI to create a comprehensive guide to aid librarians in their research work, especially those in academic settings. It enhances research skills by letting the user specify variables in prompts, generating high-quality, custom-tailored resources. The app's special feature offers a complete view of conducting and advising academic research, ranging from the basics to complex issues like research ethics and digital databases usage. Its singularity lies in the focus on librarians' research skill elevation, with extensive details on academic research.

To run this app online: [Librarian Academic Research Aide Online](https://hero.page/app/librarian-academic-research-aide-comprehensive-academic-research-guide/BXIPhDLYEvwGoGwydiEP)

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
npx hero run ./librarian_academic_research_aide.heroml
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
hero run ./librarian_academic_research_aide.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./librarian_academic_research_aide.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./librarian_academic_research_aide.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./librarian_academic_research_aide.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Librarian Academic Research Aide
```
Your task is to write a "Research Guide" for the "Academic & University" industry, specifically targeting "Librarians". Let's start by writing a comprehensive introduction that describes the purpose, content, and relevance of the guide in the academic sector.

Here's some more context about the Research Guide:
Guide Purpose Content Relevance: {{guide_purpose_content_relevance}}
Resource Variations: {{resource_variations}}
Source Credibility Assessment: {{source_credibility_assessment}}
Research Process: {{research_process}}
Research Ethics: {{research_ethics}}
Digital Libraries Databases: {{digital_libraries_databases}}
Key Terms: {{key_terms}}
Additional Materials: {{additional_materials}}

->>>>

Now we've begun the "Research Guide". We can proceed by exploring the differing types of resources which can benefit a librarian during their research. These can include but are not limited to primary and secondary, online and offline materials.

Introduction:
{{step_1}}

->>>>

We have the introduction, as well as a detailed account of the various types of resources that a librarian can use for research:

Introduction:
{{step_1}}

Resource Variations:
{{step_2}}

Next, discuss the importance of reliable and credible sources for academic research. Write a section on how to effectively evaluate the credibility and reliability of different sources.

->>>>

For our research guide, we now have a section outlining the variations of resources and another discussing how to assess source credibility:

Resource Variations:
{{step_2}}

Source Credibility Assessment:
{{step_3}}

Moving forward, create a step-by-step guide on how to conduct effective academic research. This should include advice on organizing, synthesizing, and citing information accurately.

->>>>

So far in our guide, we have discussions about resource variations, source credibility assessments, and now a guide on the research process:

Source Credibility Assessment:
{{step_3}}

Research Process:
{{step_4}}

Next, discuss the ethics of academic research, including an insight on plagiarism and its consequences. This section should not solely be beneficial for librarians conducting their own research but also serve as a frame of reference for advising staff and students.

->>>>

We now have a step-by-step guide to conducting research and details on the ethics of academic research:

Research Process:
{{step_4}}

Research Ethics:
{{step_5}}

Now, let's delve into the benefits and usage of digital libraries and databases in academic research. Be sure to include information about commonly utilized databases, the understandings of changing database structures and search mechanisms.

->>>>

In our guide, we now have covered the ethics of academic research and the usage of digital libraries and databases:

Research Ethics:
{{step_5}}

Digital Libraries & Databases:
{{step_6}}

Conclude the research guide with a summary that reinforces its purpose. In this summary, reiterate how effectively utilizing the guide can enhance a librarian's research skills.

->>>>

After discussing digital libraries and databases, we now have a conclusion that reinforces the purpose of the guide:

Digital Libraries & Databases:
{{step_6}}

Conclusion:
{{step_7}}

Now, consider creating a glossary of key terms often used in academic research. This will facilitate the librarian's understanding of uncommon or complex terms.

->>>>

Our research guide now has a conclusion and a glossary of key terms:

Conclusion:
{{step_7}}

Glossary:
{{step_8}}

Finally, compile a section that provides additional reading, references, or links to recommended books, journals, and websites. This would serve to increase the librarian's knowledge base.


```

