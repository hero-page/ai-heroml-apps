# Librarian Guide AI Composer

Explore the academic library space with Librarian Guide AI Composer—your virtual, AI-powered academic librarian guide. Seamlessly specify variables in prompts and generate customized, high-quality content. Learn about the primary roles and responsibilities of librarians, cataloging processes, the use of online systems for research, and all about the check-in and check-out of materials. Get insight on conducting library tours, community outreach, managing resource allocation and digital errors. Concludes with a librarian's essential role summary and points to additional resources—specialized content for librarians in academia.

To run this app online: [Librarian Guide AI Composer Online](https://hero.page/app/librarian-guide-ai-composer-ai-powered-academic-librarian-guide/nait8Sm8zK0toooO2wVB)

[![Run Librarian Guide AI Composer Online](/assets/run.svg)](https://hero.page/app/librarian-guide-ai-composer-ai-powered-academic-librarian-guide/nait8Sm8zK0toooO2wVB)

To learn more about AI Apps for Librarian use-cases in the Academic & University industry, read [How to Enhance Library Workflows with AI Technology](https://hero.page/blog/ai/academic-and-university/how-to-enhance-library-workflows-with-ai-technology/170706)

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
npx hero run ./librarian_guide_ai_composer.heroml
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
hero run ./librarian_guide_ai_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./librarian_guide_ai_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./librarian_guide_ai_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./librarian_guide_ai_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Librarian Guide AI Composer
```
Let's start with writing an overview that explains the primary role and responsibilities of a librarian: {{librarian_responsibilities}}.

Here's some more context about the User Instructions:
Librarian Responsibilities: {{librarian_responsibilities}}
Cataloging Procedures: {{cataloging_procedures}}
Online System: {{online_system}}
Circulation Operations: {{circulation_operations}}
Patron Service: {{patron_service}}
Special Services: {{special_services}}
Common Issues: {{common_issues}}
Librarian Role: {{librarian_role}}

->>>>

For the user instructions for a librarian in the academic industry, we have an overview that explains the primary role and responsibilities:

Overview of Librarian Responsibilities:
{{step_1}}

Next, let's present a step-by-step guide for cataloging and classifying materials such as books, films, and publications: {{cataloging_procedures}}.

->>>>

In addition to the primary roles and responsibilities of a librarian:

Overview of Librarian Responsibilities:
{{step_1}}

We also have a step-by-step guide for cataloging and classifying materials:

Cataloging and Classifying Guide:
{{step_2}}

Now, detail the system and structure of the online cataloging and research system, focusing on how to navigate and use it: {{online_system}}.

->>>>

In our user instructions, apart from explaining primary roles, and cataloging and classifying guide,

Overview of Librarian Responsibilities:
{{step_1}}

Cataloging and Classifying Guide:
{{step_2}}

We also have detailed the online cataloging and research system:

Online Cataloging and Research System:
{{step_3}}

Next, provide instructions on managing circulation operations, such as how to check materials in and out, re-shelving, and handling holds and interlibrary loans: {{circulation_operations}}.

->>>>

Our user instructions for a librarian so far includes:

Cataloging and Classifying Guide:
{{step_2}}

Online Cataloging and Research System:
{{step_3}}

We now have instructions for managing circulation operations:

Circulation Operations Guide:
{{step_4}}

Proceed to discuss the protocols and procedures for dealing with patron questions and providing reference services: {{patron_service}}.

->>>>

Thus far, our user instructions coverage includes:

Online Cataloging and Research System:
{{step_3}}

Circulation Operations Guide:
{{step_4}}

We now have guidelines on patron service:

Patron Service Guide:
{{step_5}}

Next, explain the guidelines for handling special services such as library tours, literary programs, or community outreach: {{special_services}}.

->>>>

We have instructions on:

Circulation Operations Guide:
{{step_4}}

Patron Service Guide:
{{step_5}}

We also have guidelines on handling of special services:

Special Services Guide:
{{step_6}}

Now, offer tips and solutions for common issues or difficulties a librarian may encounter in their daily work, including conflict management, resource allocation, and digital system errors: {{common_issues}}.


```

