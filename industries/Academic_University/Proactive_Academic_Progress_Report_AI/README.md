# Proactive Academic Progress Report AI

Proactive Academic Progress Report AI, an AI-Based Personalized Academic Guidance app, enables users to specify variables in prompts for detailed, bespoke academic progress reports. Harnessing the power of advanced AI, it creates top-quality, individualized content for students. Your comprehensive evaluation includes subjects performance, GPA, standing, and credits earned. Additionally, it scrutinizes performance trends, academic goals and offers valuable feedback plus course recommendations. Unlike standard progress reports, this app adds value by offering an insightful analysis and personalized advice based on the student's aspirations. Highlighting the next steps and advisor contacts, this tool aims to proactively guide students towards academic success.

To run this app online: [Proactive Academic Progress Report AI Online](https://hero.page/app/proactive-academic-progress-report-ai-ai-based-personalized-academic-guidance/NeyzqwHxRU7TSI7mQVf5)

[![Run Proactive Academic Progress Report AI Online](/assets/run.svg)](https://hero.page/app/proactive-academic-progress-report-ai-ai-based-personalized-academic-guidance/NeyzqwHxRU7TSI7mQVf5)

To learn more about AI Apps for Academic Advisor use-cases in the Academic & University industry, read [How to Streamline Academic Advising with AI Tools](https://hero.page/blog/ai/academic-and-university/how-to-streamline-academic-advising-with-ai-tools/170708)

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
npx hero run ./proactive_academic_progress_report_ai.heroml
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
hero run ./proactive_academic_progress_report_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./proactive_academic_progress_report_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./proactive_academic_progress_report_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./proactive_academic_progress_report_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Proactive Academic Progress Report AI
```
Your task is to write an "Academic Progress Report" for the "Academic & University" industry, specifically for an "Academic Advisor". 

Let's begin by creating an overview that provides context for the specific academic period: {{academic_period}} the report covers.

Here's some more context about the Academic Progress Report:
Academic Period: {{academic_period}}
Student Name: {{student_name}}
Student Major: {{student_major}}
Academic Standing: {{academic_standing}}

->>>>

We are creating an "Academic Progress Report", and we have a context for the academic period:

Academic Period:
{{step_1}}

Now, write an introduction that mentions the student's name: {{student_name}}, along with their major/concentration: {{student_major}} to personalize the report.

->>>>

In our "Academic Progress Report" covering the following period:

Academic Period:
{{step_1}}

We have a personalized introduction:

Introduction:
{{step_2}}

Next, discuss the student's academic performance by detailing the individual subjects/courses they have undertaken in the mentioned academic period. Include grades, noteworthy improvements or setbacks, and brief comments on participation or notable achievements.

->>>>

In the "Academic Progress Report" with the following introduction:

Introduction:
{{step_2}}

We captured the student's performance in the following way:

Academic Performance:
{{step_3}}

Following that, write a Progress Assessment section that provides the cumulative GPA, standing within the program: {{academic_standing}}, and the number of credits achieved associated with the student's name.

->>>>

The "Academic Progress Report" with its discussion of academic performance is as follows:

Academic Performance:
{{step_3}}

And, we've compiled the Progress Assessment:

Progress Assessment:
{{step_4}}

We now need to add a section on Performance Trends where you provide an analysis of the student's progress over multiple periods, not just the current academic period. Compare the current performance with past performance, noting any trends, improvements, or areas of concern.

->>>>

In our "Academic Progress Report", we have the following sections so far:

Progress Assessment:
{{step_4}}

And we've analyzed Performance Trends:

Performance Trends:
{{step_5}}

Now, discuss the student's Academic Goals that have been set for the academic period, noting if they were achieved and how successfully. Mention the student's broader education goals, and how their current progress aligns with these goals.

->>>>

In our "Academic Progress Report", we have:

Performance Trends:
{{step_5}}

And we've discussed the Academic Goals:

Academic Goals:
{{step_6}}

Let's now create a Future Planning section where you provide constructive feedback and suggest future course enrollments, academic resources, or any skill development programs that would help to improve the student's success rate. This recommendation part should correlate with the student's educational goals and their major.

->>>>

For our "Academic Progress Report", we have:

Academic Goals:
{{step_6}}

And we have provided Future Planning:

Future Planning:
{{step_7}}

Now, conclude with a summary of all major points discussed in the report, provide the next steps for the students, advisors, or any other relevant party.

->>>>

In our "Academic Progress Report", to go with our:

Future Planning:
{{step_7}}

We have a conclusion:

Conclusion:
{{step_8}}

Do not forget to include contact information for the academic advisor in case the student or other stakeholders have questions or need further discussion on the report.


```

