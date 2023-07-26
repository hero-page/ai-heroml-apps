# TA Feedback & Improvement Generator

The TA Feedback & Improvement Generator app uses advanced AI to create detailed, comprehensive evaluation reports for Teaching Assistants. Users can specify variables to tailor feedback around classroom experiences and industry-specific requirements, generating constructive criticism and improvement suggestions. The unique attribute of this AI-powered TA Evaluation tool is its emphasis on politeness, going beyond general feedback to offer in-depth, role-specific input for academic or university settings.

To run this app online: [TA Feedback & Improvement Generator Online](https://hero.page/app/ta-feedback-and-improvement-generator-ai-powered-ta-evaluation-and-advancement/ScnRmoX1ecOS1Rozc2Ts)

[![Run TA Feedback & Improvement Generator Online](/assets/run.svg)](https://hero.page/app/ta-feedback-and-improvement-generator-ai-powered-ta-evaluation-and-advancement/ScnRmoX1ecOS1Rozc2Ts)

To learn more about AI Apps for Teaching Assistant use-cases in the Academic & University industry, read [How to Enhance University Teaching with AI Tools for Tutorials, Rubrics, and Feedback](https://hero.page/blog/ai/academic-and-university/how-to-enhance-university-teaching-with-ai-tools-for-tutorials-rubrics-and-feedback/170705)

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
npx hero run ./ta_feedback_and_improvement_generator.heroml
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
hero run ./ta_feedback_and_improvement_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ta_feedback_and_improvement_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ta_feedback_and_improvement_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ta_feedback_and_improvement_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for TA Feedback & Improvement Generator
```
Here is your task to create a "Student Feedback" for a "Teaching Assistant" in the "Academic & University" industry. 
Let's start by writing an introduction that states the purpose of the feedback and provides context for your relationship with the {{teaching_assistant}}.

Here's some more context about the Student Feedback:
Teaching Assistant: {{teaching_assistant}}
Specific Instance 1: {{specific_instance_1}}
Specific Instance 2: {{specific_instance_2}}

->>>>

Now, you have the introduction for your "Student Feedback":

Introduction:
{{step_1}}

Next, write an overall assessment of the {{teaching_assistant}}, including highlighting their strengths.

->>>>

With the introduction and overall assessment complete, this is your feedback so far:

Introduction:
{{step_1}}

Overall Assessment:
{{step_2}}

Moving forward, provide specific experiences from your classroom with the {{teaching_assistant}}. Mention their helpfulness, clarity in explanations, availability for discussions, responsiveness, and interaction.

->>>>

Now you have an introduction, an overall assessment, and a detailed account of your experiences. Here is your current feedback:

Introduction:
{{step_1}}

Overall Assessment:
{{step_2}}

Specific Experiences:
{{step_3}}

For the next step, detail how the {{teaching_assistant}} has helped in enhancing your understanding of the academic subject matter.

->>>>

Now, this is your feedback: 

Introduction:
{{step_1}}

Overall Assessment:
{{step_2}}

Specific Experiences:
{{step_3}}

Teaching Capability:
{{step_4}}

Now, let's give constructive criticism. Remember, not all feedback is positive; however, it should be constructive and assist the {{teaching_assistant}} in understanding the areas of improvement.

->>>>

We have the feedback's Introduction, Overall Assessment, Specific Experiences, Teaching Capability, and now a section on constructive criticism:

Introduction:
{{step_1}}

Overall Assessment:
{{step_2}}

Specific Experiences:
{{step_3}}

Teaching Capability:
{{step_4}}

Constructive Criticism:
{{step_5}}

Moving on, suggest actions which the {{teaching_assistant}} might consider to improve future learning experiences.

->>>>

Now you have added recommendations to your feedback:

Introduction:
{{step_1}}

Overall Assessment:
{{step_2}}

Specific Experiences:
{{step_3}}

Teaching Capability:
{{step_4}}

Constructive Criticism:
{{step_5}}

Recommendations:
{{step_6}}

To conclude the feedback, let's sign off politely. Write a closing statement that includes a final expression of appreciation for the TA's efforts.


```

