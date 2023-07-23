# Academic Requirement AI Guide

Academic Requirement AI Guide is an innovative app aiding students throughout their academic journey. Its AI-driven architecture generates a detailed report encompassing key details like degree offerings, general and elective requirements, progress tracking and GPA guidelines, tailored for specific academic programs. It nurtures regular interaction with advisors and highlights potential career opportunities. This comprehensive tool is designed to equip students for successful degree completion.

To run this app online: [Academic Requirement AI Guide Online](https://hero.page/app/academic-requirement-ai-guide-ai-powered-comprehensive-academic-guide/W1aHQunWMg2cz9mtfqLE)

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
npx hero run ./academic_requirement_ai_guide.heroml
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
hero run ./academic_requirement_ai_guide.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_requirement_ai_guide.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_requirement_ai_guide.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_requirement_ai_guide.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Requirement AI Guide
```
Your task is to write a "Degree Requirement Overview" for the "Academic & University" industry, specifically for a "Academic Advisor". 
First, generate a brief introduction explaining the purpose of the "Degree Requirement Overview", which is to provide {{academic_program}} requirements applicable for the current academic year.

Here's some more context about the Degree Requirement Overview:
Academic Program: {{academic_program}}
Academic Department: {{academic_department}}

->>>>

Your Degree Requirement Overview so far is:

Introduction:
{{step_1}}

For the first segment, list down all the degree programs offered under the {{academic_department}}. Mention the degree offerings such as Bachelor's, Master's, or Doctorate for each program and explain the main objectives of each degree.

->>>>

Your Degree Requirement Overview so far is:

Introduction:
{{step_1}}

Degree Programs:
{{step_2}}

For the next segment, highlight the "General Education Requirements". These are the courses that every student must complete, regardless of their major. Include basic skills courses, humanities, social and behavioral science courses, mathematics, natural science, and language courses that must be completed to fulfill the general education requirements.

->>>>

Your Degree Requirement Overview has:

Degree Programs:
{{step_2}}

General Education Requirements:
{{step_3}}

In the following segment, titled "Major-Specific Requirements", clearly indicate the number of credit hours and specific courses required for each program within the {{academic_department}}. This will include both lower division and upper division courses. Include prerequisites for each course if applicable.

->>>>

So far, The Degree Requirement Overview contains:

General Education Requirements:
{{step_3}}

Major-Specific Requirements:
{{step_4}}

Dedicate the next segment to "Elective Requirements". These are courses that students may choose according to their interest but must be within certain guidelines to meet the degree requirements.

->>>>

Your Degree Requirement Overview now contains:

Major-Specific Requirements:
{{step_4}}

Elective Requirements:
{{step_5}}

In the subsequent segment, "Academic Progress and GPA Requirements", outline the academic standing protocols, detailing what is considered good academic standing and when a student is at risk due to poor grades or not meeting other academic policies.

->>>>

We have these segments in our Degree Requirement Overview document so far:

Elective Requirements:
{{step_5}}

Academic Progress and GPA Requirements:
{{step_6}}

End this document with a conclusion that emphasizes the importance of meeting these requirements for successful degree completion in the {{academic_program}}. This could also include a brief note encouraging students to meet regularly with their academic advisors.

->>>>

Our overview now has:

Academic Progress and GPA Requirements:
{{step_6}}

Conclusion:
{{step_7}}

For added industry-specific value, generate a segment titled "Career Opportunities" where students may get an overview of the potential job roles, industries, and company types that frequently hire graduates in their field of study.


```

