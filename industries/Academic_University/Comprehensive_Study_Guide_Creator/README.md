# Comprehensive Study Guide Creator

As an AI-powered undergraduate study aid, Comprehensive Study Guide Creator enables you to detail variables in study prompts for customized, high-quality content. Tailoring each guide, this app ensures comprehensive coverage of course topics with in-depth details, concrete real-world applications, and self-assessment sections per topic. Review key takeaways, captured in content summaries, and conclude your study with a brief, yet comprehensive review of the guide. This study aid delivers not only academic insights but ensures enhanced understanding and application of knowledge for undergraduate students.

To run this app online: [Comprehensive Study Guide Creator Online](https://hero.page/app/comprehensive-study-guide-creator-ai-powered-undergraduate-study-aid/TLRkq600Os73FSGtddg7)

[![Run Comprehensive Study Guide Creator Online](/assets/run.svg)](https://hero.page/app/comprehensive-study-guide-creator-ai-powered-undergraduate-study-aid/TLRkq600Os73FSGtddg7)

To learn more about AI Apps for Undergraduate Student use-cases in the Academic & University industry, read [How to Ace University Writing with AI Academic Assistance](https://hero.page/blog/ai/academic-and-university/how-to-ace-university-writing-with-ai-academic-assistance/170701)

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
npx hero run ./comprehensive_study_guide_creator.heroml
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
hero run ./comprehensive_study_guide_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./comprehensive_study_guide_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./comprehensive_study_guide_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./comprehensive_study_guide_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Comprehensive Study Guide Creator
```
Let's prepare a "Study Guide" for the "Academic & University" industry for an "Undergraduate Student". Let's start by writing an introductory paragraph summarizing the main aim of the study guide: {{study_aim}}.

Here's some more context about the Study Guide:
Study Aim: {{study_aim}}
Course Topics: {{course_topics}}
Topic Overview: {{topic_overview}}
Specific Topic Facts: {{specific_topic_facts}}
Industry Application: {{industry_application}}
Specific Topic Questions: {{specific_topic_questions}}
Topic Takeaways: {{topic_takeaways}}

->>>>

Now we have an introduction for our study guide, which explains its purpose:

Introduction:
{{step_1}}

Next, let's create a syllabus outline that lists the various topics and subtopics to be covered within the course.

->>>>

We now have a syllabus outline:

Syllabus Outline:
{{step_2}}

Based on this outline, let's expand on each topic in individual sections. Each section should start with an overview of the topic and outline key points, theories, facts, or formulas that are critical to understanding the particular topic.

->>>>

We now have detailed sections for each topic:

Individual Topic Sections:
{{step_3}}

For each topic, let's now provide a section dedicated to explaining any available real-world application or industry relevance.

->>>>

Now we have industry and real-world applications for each topic:

Industry and Real-World Applications:
{{step_4}}

Let's continue by including a section for self-assessment after every topic. This could include multiple choice questions, fill in the blanks, or short answer questions.

->>>>

We now have a self-assessment section for each topic:

Self-assessment Sections:
{{step_5}}

Next, let's conclude each topic section with a brief summary capturing key takeaways.


```

