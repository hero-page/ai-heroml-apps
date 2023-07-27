# Kids Study Guide Creator AI

Kids Study Guide Creator AI offers a smart, personalized learning experience for children. This AI-powered app lets you input variables to generate a comprehensive, age-friendly guide for young learners. It breaks down any subject into digestible chapters, provides succinct summaries and keywords, deciphers terms in kid-friendly language, and includes assessment through Q&A. It offers safe resources for extensive learning and a final review section with an answer key. Tailored to enhance children's learning, this app offers structured, easy-to-understand, age-appropriate information.

To run this app online: [Kids Study Guide Creator AI Online](https://hero.page/app/kids-study-guide-creator-ai-customized-ai-powered-kids-learning/vna9zpwhve4ic0rW9acw)

[![Run Kids Study Guide Creator AI Online](/assets/run.svg)](https://hero.page/app/kids-study-guide-creator-ai-customized-ai-powered-kids-learning/vna9zpwhve4ic0rW9acw)

To learn more about AI Apps for Educational Author use-cases in the Children's Books & Learning Materials industry, read [How to Streamline Children's Book Writing and Learning with AI](https://hero.page/blog/ai/children's-books-and-learning-materials/how-to-streamline-children's-book-writing-and-learning-with-ai/170777)

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
npx hero run ./kids_study_guide_creator_ai.heroml
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
hero run ./kids_study_guide_creator_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./kids_study_guide_creator_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./kids_study_guide_creator_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./kids_study_guide_creator_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Kids Study Guide Creator AI
```
Your task is to write a "Study Guide" for the "Children's Books & Learning Materials" industry, specifically for an "Educational Author". 

Let's start with an introduction that provides an overview of the subject matter: {{subject_matter}}. 

Here's some more context about the Study Guide:
Subject Matter: {{subject_matter}}

->>>>

Our "Study Guide" has begun with an introduction:

Introduction:
{{step_1}}

Now, let's break down this {{subject_matter}} into Chapters or Units. Each chapter should correlate to a major concept or topic related to the {{subject_matter}}.

->>>>

For our "Study Guide", we have divided the {{subject_matter}} into chapters:

Chapters/Units:
{{step_2}}

Next, for every chapter/unit, we will begin with a summary that highlights key points and ideas in simple, age-appropriate language.

->>>>

Our "Study Guide" has chapter summaries:

Chapter Summaries:
{{step_3}}

Let's now generate a list of keywords or terms for each chapter/unit. This list should be directly related to the major concept of the chapter/unit from the {{subject_matter}}.

->>>>

We have the keywords or terms listed for each chapter/unit of {{subject_matter}}:

Keywords/Terms:
{{step_4}}

It's time to include simplified definitions or explanations for the keywords/terms list.

->>>>

Our "Study Guide" now includes definitions of the listed terms: 

Definitions:
{{step_5}}

Next, we need to create a series of questions related to each chapter or unit. The questions should measure the understanding of the child regarding the major concepts presented in the chapter/unit of the {{subject_matter}}.

->>>>

We now have sets of questions pertaining to each chapter/unit of our {{subject_matter}}:

Questions:
{{step_6}}

With each question, let's provide detailed answers or solutions. The aim is to guide the child's understanding and reinforce the concepts of the {{subject_matter}}.

->>>>

We have now prepared answers to our questions, supporting comprehension of the {{subject_matter}}:

Answers:
{{step_7}}

At this stage, we'll inject a section for 'Additional Resources or Recommended Reading.' This should include a list of books, websites or articles that further explain the {{subject_matter}}. Make sure these resources are age-appropriate and safe for children’s use.

->>>>

Our study guide now features Additional Resources that supplement understanding of the {{subject_matter}}:

Additional Resources:
{{step_8}}

Next, conclude the study guide with a comprehensive review section that revisits the major concepts of all chapters/units of the {{subject_matter}}. Include some questions covering the entire subject to test overall understanding.

->>>>

We now have a comprehensive review section that ties together all the major concepts of our {{subject_matter}}:

Comprehensive Review:
{{step_9}}

Lastly, we need to create an answer key for all the questions in the review section. This will enable students and parents to check answers and understanding of the entire {{subject_matter}}. 


```

