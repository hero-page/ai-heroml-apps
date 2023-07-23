# Academic Advisor Course Guide AI

The Academic Advisor Course Guide AI is a revolutionary app designed for the Academic & University industry. It uses advanced AI to create tailor-made content, including detailed course descriptions, sample degree plans, prerequisites, and FAQs about course selection. This app is not a generic guide; it's designed specifically for academic advisors, providing comprehensive information to make advising tasks simpler and more effective. With this, advisors can guide students to make smarter course selections. Get ready for improved efficiency and precision in course advising.

To run this app online: [Academic Advisor Course Guide AI Online](https://hero.page/app/academic-advisor-course-guide-ai-ai-powered-university-course-advisor/4ewbHSymxXl0kulk8Mpn)

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
npx hero run ./academic_advisor_course_guide_ai.heroml
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
hero run ./academic_advisor_course_guide_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academic_advisor_course_guide_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academic_advisor_course_guide_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academic_advisor_course_guide_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academic Advisor Course Guide AI
```
First, create an introduction to the "Course Selection Guide". The introduction should include a brief explanation of the guide's purpose and its importance in the "Academic & University" industry, specifically for an "Academic Advisor". 

Here's some more context about the Course Selection Guide:
Guide Purpose: {{guide_purpose}}
Academic Department: {{academic_department}}
Course Description: {{course_description}}
Degree Plan: {{degree_plan}}
Course Prerequisites: {{course_prerequisites}}
FAQs: {{FAQs}}
Contact Information: {{contact_information}}

->>>>

Now we have the introduction for our "Course Selection Guide":

Introduction:
{{step_1}}

Next, provide specifics for each course. The details should include the course name, course code, description, prerequisites, co-requisites, and credit hours. These should be presented according to the identified academic department or another logical order that fits the institution.

->>>>

The "Course Selection Guide" currently contains:

Introduction:
{{step_1}}

Course Details:
{{step_2}}

Moving forward, for each course, elaborate on the description. Highlight the topics covered, learning outcomes, and the teaching method, whether lecture-based, lab-based, or a mix of both.

->>>>

Now, the "Course Selection Guide" has:

Introduction:
{{step_1}}

Course Details:
{{step_2}}

Expanded Course Descriptions:
{{step_3}}

Afterwards, create a degree plan showing the sequence of courses taken each semester to complete a particular degree program. Customize this plan based on full-time and part-time options, and any specialties within the degree.

->>>>

The "Course Selection Guide" currently comprises:

Introduction:
{{step_1}}

Course Details:
{{step_2}}

Expanded Course Descriptions:
{{step_3}}

Degree Plan:
{{step_4}}

Next, compile information about pre- and co-requisites for each course. This will assist students in planning their course sequences effectively.

->>>>

The "Course Selection Guide" includes the following sections:

Introduction:
{{step_1}}

Course Details:
{{step_2}}

Expanded Course Descriptions:
{{step_3}}

Degree Plan:
{{step_4}}

Course Pre- and Co-Requisites:
{{step_5}}

After that, make a list of frequently asked questions with their corresponding answers to address any common questions or concerns students may have about course selection.

->>>>

The "Course Selection Guide" now contains:

Introduction:
{{step_1}}

Course Details:
{{step_2}}

Expanded Course Descriptions:
{{step_3}}

Degree Plan:
{{step_4}}

Course Pre- and Co-Requisites:
{{step_5}}

FAQ Section:
{{step_6}}

To conclude the guide, provide the contact information of advisors, departments, or other resources students can reach out to for further assistance.


```

