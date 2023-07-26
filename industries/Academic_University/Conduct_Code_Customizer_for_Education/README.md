# Conduct Code Customizer for Education

Introducing Conduct Code Customizer for Education, your reliable partner for crafting tailored conduct codes. Empowered by AI, the app lets you precisely specify your institution's requirements, for a comprehensive, customized Student Conduct Code. The AI considers your institution's unique identity and values, crafting conduct codes that employ expected behavior, rules, student rights and more. The result? A conduct code that fosters a productive learning environment and routinely updates as your institution grows.

To run this app online: [Conduct Code Customizer for Education Online](https://hero.page/app/conduct-code-customizer-for-education-tailored-conduct-codes-via-ai/z08qgDDIlrhbbi4PvBE6)

[![Run Conduct Code Customizer for Education Online](/assets/run.svg)](https://hero.page/app/conduct-code-customizer-for-education-tailored-conduct-codes-via-ai/z08qgDDIlrhbbi4PvBE6)

To learn more about AI Apps for Student Affairs Officer use-cases in the Academic & University industry, read [How to Innovate Academic Planning with AI Tools](https://hero.page/blog/ai/academic-and-university/how-to-innovate-academic-planning-with-ai-tools/170709)

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
npx hero run ./conduct_code_customizer_for_education.heroml
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
hero run ./conduct_code_customizer_for_education.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./conduct_code_customizer_for_education.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./conduct_code_customizer_for_education.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./conduct_code_customizer_for_education.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Conduct Code Customizer for Education
```
Your task is to write a "Student Conduct Code" for the "Academic & University" industry, specifically for a "Student Affairs Officer". 

Let's start by writing an introduction that clearly outlines the importance and purpose of the Conduct Code in promoting a conducive learning environment.

Here's some more context about the Student Conduct Code:
Purpose Of Code: {{purpose_of_code}}
Behavior Expectation: {{behavior_expectation}}
Categories Of Rules: {{categories_of_rules}}
Disciplinary Actions: {{disciplinary_actions}}
Student Rights: {{student_rights}}
Reporting Procedure: {{reporting_procedure}}
Policy Updates: {{policy_updates}}

->>>>

We are creating a "Student Conduct Code" and we have written an introduction:

Introduction:
{{step_1}}

Next, we will write a section that details the overall expectations for student behavior. This might include broad guidelines around respect, honesty, and integrity within the academic community.

->>>>

We are creating a "Student Conduct Code", and we have outlined our expectations for student behavior:

Introduction:
{{step_1}}

Behavior Expectations:
{{step_2}}

Now let's write a comprehensive list of specific rules and regulations for students. We will break these down into categories, and provide simple and concise instructions and descriptions of acceptable conduct under each.

->>>>

We are creating our "Student Conduct Code", and have composed a list of specific rules:

Introduction:
{{step_1}}

Behavior Expectations:
{{step_2}}

Rules and Regulations:
{{step_3}}

Next, let's detail the consequences of violating the "Student Conduct Code". This section should explain the disciplinary actions that may be taken, and how these decisions are made in a fair, impartial process.

->>>>

We're compiling our "Student Conduct Code" and we've completed a section detailing consequences for violations:

Introduction:
{{step_1}}

Behavior Expectations:
{{step_2}}

Rules and Regulations:
{{step_3}}

Consequences:
{{step_4}}

Now, include a segment about student rights, such as rights to free speech, privacy, and appeal processes.

->>>>

Our "Student Conduct Code" is taking shape, we've now incorporated a segment on student rights:

Introduction:
{{step_1}}

Behavior Expectations:
{{step_2}}

Rules and Regulations:
{{step_3}}

Consequences:
{{step_4}}

Student Rights:
{{step_5}}

Subsequently, let's add a section that explains the process for reporting violations and seeking guidance.

->>>>

We're creating our "Student Conduct Code", and we have outlined the reporting procedure:

Introduction:
{{step_1}}

Behavior Expectations:
{{step_2}}

Rules and Regulations:
{{step_3}}

Consequences:
{{step_4}}

Student Rights:
{{step_5}}

Reporting Procedure:
{{step_6}}

Next, outline any industry or institution-specific rules. For instance, these might vary depending on whether the institution is a physical campus or an online university, or a technical program vs a liberal arts program.

->>>>

We're completing our "Student Conduct Code", with inclusion of industry-specific rules:

Introduction:
{{step_1}}

Behavior Expectations:
{{step_2}}

Rules and Regulations:
{{step_3}}

Consequences:
{{step_4}}

Student Rights:
{{step_5}}

Reporting Procedure:
{{step_6}}

Institution-specific Rules:
{{step_7}}

As the final step, include a reminder or process that the Student Conduct Code should be regularly reviewed and updated based on changes in institutional policies, laws, or student needs.


```

