# ProfGuide: Precision Lecture Planner

ProfGuide: Precision Lecture Planner is an innovative AI-powered app that crafts detailed lecture notes for academic professionals. Users can specify variables in prompts for customizability. This app stands out by generating inclusive content with deeper insights. Its notes go beyond summarizing lectures, including objectives, topic walkthroughs, misconception handling, key point summaries, discussion questions, and introduction to the next topic. The app enhances interactive learning and offers notes in an easy-to-understand, academic language.

To run this app online: [ProfGuide: Precision Lecture Planner Online](https://hero.page/app/profguide:-precision-lecture-planner-ai-powered-comprehensive-lecture-notes/nzTE4cYYxndDwQhj3ZMv)

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
npx hero run ./profguide_precision_lecture_planner.heroml
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
hero run ./profguide_precision_lecture_planner.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./profguide_precision_lecture_planner.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./profguide_precision_lecture_planner.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./profguide_precision_lecture_planner.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for ProfGuide: Precision Lecture Planner
```
Your task is to write "Lecture Notes" for the "Academic & University" industry, specifically for a "Professor". 

Let's get started by creating an overview that outlines the lecture's main objective or focus: {{lecture_objective}}. This would help students understand the relevance and importance of the lecture material.

Here's some more context about the Lecture Notes:
Lecture Objective: {{lecture_objective}}
Main Topics: {{main_topics}}
Next Topic: {{next_topic}}

->>>>

To begin writing our lecture notes, we have produced an overview:

Overview:
{{step_1}}

Next, introduce the main themes or topics that will be covered in the lecture: {{main_topics}}. This will help students follow the progression of the lecture and understand how different parts relate to each other.

->>>>

Having crafted the overview:

Overview:
{{step_1}}

We have also highlighted the main themes that will be discussed:

Main Themes:
{{step_2}}

Now detail a step-by-step process explicitly covering each of the main topics: {{main_topics}}. Start with the basic principles before moving on to complex concepts. Provide ample examples and simple explanations for enhanced understanding.

->>>>

Our lecture notes so far state the overview and main themes:

Overview:
{{step_1}}

Main Themes:
{{step_2}}

And now, we have a detailed step-by-step process for the topics:

Step-by-step Process:
{{step_3}}

Importantly, incorporate a segment dedicated to addressing common misconceptions and clarifying tricky or confusing concepts related to the {{main_topics}}.

->>>>

We're making progress with the lecture notes:

Step-by-step Process:
{{step_3}}

And we've now created a section to address common misconceptions about the topics:

Common Misconceptions and Clarifications:
{{step_4}}

Next, conclude with a summary that consolidates the main points of the lecture, and reiterate the lecture's objective: {{lecture_objective}}.

->>>>

Our lecture notes are shaping up nicely with:

Common Misconceptions and Clarifications:
{{step_4}}

Now we have a summary that reinforces the crucial aspects of the lecture:

Summary and Objective Reiteration:
{{step_5}}

Create a section for potential questions, discussions, and/or further readings related to {{main_topics}}. This encourages students to think critically about the material.

->>>>

Our lecture notes have advanced with:

Summary and Objective Reiteration:
{{step_5}}

We created a dedicated section for questions and further readings:

Questions and Further Readings:
{{step_6}}

Lastly, provide an introduction to the topic of the next lecture: {{next_topic}}. This will help keep students interested and provide continuity in their journey.


```

