# Kids Crafts Project Feedback Generator

Kids Crafts Project Feedback Generator is an AI-powered app especially made for Hobby Instructors in the Children's Crafts & Hobbies industry. It facilitates prompt customization for unique insights and provides high-quality feedback on kid's projects. It gives an extensive analysis covering project overview, executed objectives, output evaluation, strengths, areas for improvement with solutions, and a summary. Standout feature: detailed evaluation of a distinct niche industry.

To run this app online: [Kids Crafts Project Feedback Generator Online](https://hero.page/app/kids-crafts-project-feedback-generator-ai-powered-hobby-project-evaluator/xZZdEJ4vCE7BST2G16b0)

[![Run Kids Crafts Project Feedback Generator Online](/assets/run.svg)](https://hero.page/app/kids-crafts-project-feedback-generator-ai-powered-hobby-project-evaluator/xZZdEJ4vCE7BST2G16b0)

To learn more about AI Apps for Hobby Instructor use-cases in the Children's Crafts & Hobbies industry, read [How to Elevate Children's Craft Lessons with AI Tools](https://hero.page/blog/ai/children's-crafts-and-hobbies/how-to-elevate-children's-craft-lessons-with-ai-tools/170781)

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
npx hero run ./kids_crafts_project_feedback_generator.heroml
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
hero run ./kids_crafts_project_feedback_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./kids_crafts_project_feedback_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./kids_crafts_project_feedback_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./kids_crafts_project_feedback_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Kids Crafts Project Feedback Generator
```
Your task is to write a "Project Feedback" for the "Children's Crafts & Hobbies" industry, specifically for a "Hobby Instructor". Let's start with creating an introduction that gives a general overview of the project. This should include details about its scale, scope, duration, and objectives.

Here's some more context about the Project Feedback:
Project Overview: {{project_overview}}
Objectives Execution: {{objectives_execution}}
Individual Outputs: {{individual_outputs}}
Project Strengths: {{project_strengths}}
Areas For Improvement: {{areas_for_improvement}}
Summary: {{summary}}

->>>>

We have the introduction for our "Project Feedback":

Introduction:
{{step_1}}

Now, let's have a detailed review of the project's objectives and how well they have been met. This should explore the extent to which the project's goals were met, including what was done well and what could've been done differently.

->>>>

Now, in our "Project Feedback", we have an introduction and a review of the objectives execution:

Introduction:
{{step_1}}

Objectives Execution Review:
{{step_2}}

Let's now address each output of the project individually, providing valuable feedback on them in accordance with the project criteria.

->>>>

We have reviewed the individual outputs of the project:

Introduction:
{{step_1}}

Objectives Execution Review:
{{step_2}}

Individual Outputs Review:
{{step_3}}

Next, let's discuss the strengths of the project – what worked well and what were the key achievements.

->>>>

In our "Project Feedback", we're making progress:

Introduction:
{{step_1}}

Objectives Execution Review:
{{step_2}}

Individual Outputs Review:
{{step_3}}

Project Strengths:
{{step_4}}

Moving forward, let's go ahead and highlight the areas for improvement. Offer constructive criticism and suggest ways that can make the project even more efficient or effective in the future.


```

