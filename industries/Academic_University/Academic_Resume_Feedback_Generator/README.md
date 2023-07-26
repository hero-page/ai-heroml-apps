# Academic Resume Feedback Generator

Discover the power of AI with the Academic Resume Feedback Generator app. This dedicated application caters specifically to Career Counselors in the Academic & University industry by providing an in-depth, tailored critique of professional resumes. Users set specific variables, allowing the AI to appraise the structure, content, and clarity of their resumes. This includes assessing professional experiences, academic qualifications, career objectives, and skills relevance. It gives comprehensive feedback and improvement advice, distinguishing itself with its keen focus on the academic sector.

To run this app online: [Academic Resume Feedback Generator Online](https://hero.page/app/academic-resume-feedback-generator-academic-resume-ai-critique/OJUnkSBhTXlc9fiEMOb7)

[![Run Academic Resume Feedback Generator Online](/assets/run.svg)](https://hero.page/app/academic-resume-feedback-generator-academic-resume-ai-critique/OJUnkSBhTXlc9fiEMOb7)

To learn more about AI Apps for Career Counselor use-cases in the Academic & University industry, read [How to Enhance Career Development with AI in Academia](https://hero.page/blog/ai/academic-and-university/how-to-enhance-career-development-with-ai-in-academia/170707)

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
npx hero run ./academic_resume_feedback_generator.heroml
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
hero run ./academic_resume_feedback_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_resume_feedback_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_resume_feedback_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_resume_feedback_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Resume Feedback Generator
```
Your task is to write a "Resume Feedback" for the "Academic & University" industry, specifically for a "Career Counselor". 

Let's start with a concise introduction that succinctly outlines the purpose of the feedback and briefly reflects on the overall impression of the resume.

Here's some more context about the Resume Feedback:
Introduction: {{introduction}}
Resume Structure: {{resume_structure}}
Resume Content: {{resume_content}}
Summary Evaluation: {{summary_evaluation}}
Relevant Sections Evaluation: {{relevant_sections_evaluation}}
Conclusion: {{conclusion}}

->>>>

For a "Resume Feedback" in the "Academic & University" industry for a "Career Counselor", we have the following introduction:

Introduction:
{{step_1}}

Next, commence an assessment of the resume’s structure, focusing on its readability, organization, and coherence.

->>>>

With an introduction completed, we have also analyzed the resume's structure:

Introduction:
{{step_1}}

Resume Structure Analysis:
{{step_2}}

From here, review the content of the resume, paying close attention to the clarity of the professional experiences, academic qualifications, and relevant skills. In this section, give specific examples from the resume where improvements can be made.

->>>>

We have an analysis of both the structure and content of the resume:

Structure Analysis:
{{step_2}}

Content Analysis:
{{step_3}}

Now, let's critique the 'Summary' or 'Career Objective' section of the resume, ensuring it is appropriately tailored for roles in the academic and university sphere and offers a compelling professional snapshot of the candidate.

->>>>

The introduction, structure, and content of the resume have been analyzed. In addition, we've critiqued the 'Summary' or 'Career Objective' section:

Content Analysis:
{{step_3}}

Summary or Career Objective Evaluation:
{{step_4}}

Next, evaluate the relevance and suitability of the 'Education', 'Experience', and 'Skills' sections, which are vital in the academic and university industry. Ensure they are accurate and tailored to match the specific career objectives of the candidate.


```

