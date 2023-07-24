# AI Teaching Assistant Rubric Creator

Boost your grading process with the AI Teaching Assistant Rubric Creator. Perfect for Academic & University sector, this app leverages artificial intelligence to generate clear, comprehensive assessment rubrics. Simply specify your course-specific variables and watch as the AI generates a unique rubric featuring multiple assessment criteria and detailed performance levels. Each criterion has point allocations for exceeding, meeting, or falling short of expectations. The rubric encourages academic integrity, provides room for feedback, and aligns with your course's goals. The easily understood language and transparent approach prepare students for success, and the robust, adaptable format allows for easy future updates. It's a revolution in efficient and effective grading.

To run this app online: [AI Teaching Assistant Rubric Creator Online](https://hero.page/app/ai-teaching-assistant-rubric-creator-ai-powered-university-grading-rubric/YLA0EBtg1ge9TTMckIn0)

To learn more about AI Apps for Teaching Assistant use-cases in the Academic & University industry, read [How to Enhance University Teaching with AI Tools for Tutorials, Rubrics, and Feedback](https://hero.page/blog/academic-and-university/teaching-assistant/how-to-enhance-university-teaching-with-ai-tools-for-tutorials-rubrics-and-feedback/170705)

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
npx hero run ./ai_teaching_assistant_rubric_creator.heroml
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
hero run ./ai_teaching_assistant_rubric_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ai_teaching_assistant_rubric_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ai_teaching_assistant_rubric_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ai_teaching_assistant_rubric_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for AI Teaching Assistant Rubric Creator
```
Your task is to write a "Marking Rubric" for the "Academic & University" industry, specifically for a "Teaching Assistant". 

Let's begin by outlining the purpose of this "Marking Rubric". Also, describe the course or application it's being used for: {{course_name}}. Provide some background information to contextualize its use. 

Here's some more context about the Marking Rubric:
Course Name: {{course_name}}

->>>>

We have outlined the purpose of our "Marking Rubric" and provided background on the course:

Purpose and Course Description: 
{{step_1}}

Next, define multiple criteria or tasks for assessment. 
These criteria should relate directly to the required skills, knowledge, or understanding expected from students in {{course_name}}. The criteria could include specific assignments, projects, participation level, etc.

->>>>

We have a purpose and assessment criteria for our "Marking Rubric":

Purpose and Course Description: 
{{step_1}}

Assessment Criteria: 
{{step_2}}

Now, assign performance levels to each criterion defined earlier. 
Consider classifying performance into at least 3 categories: "Exceeds Expectations," "Meets Expectations," and "Does not Meet Expectations".

->>>>

At this point, we have established the assessment criteria and performance levels:

Assessment Criteria: 
{{step_2}}

Performance Levels: 
{{step_3}}

Next, write a clear description of what each performance level entails for each criterion. 
Remember that these descriptions will guide your grading and should align with the nature of the course or assignment: {{course_name}}.

->>>>

We now have descriptions for each performance level under each criterion:

Assessment Criteria: 
{{step_2}}

Performance Levels and Descriptions: 
{{step_4}}

Assign points or percentage weights to each performance level under each criterion. 
This will form the basis of the student's overall course score in {{course_name}}.

->>>>

So far, we've defined criteria, performance levels, descriptions, and adopted a scoring scheme:

Performance Levels, Descriptions, and Scoring: 
{{step_5}}

Next, provide an explanation of how to use the rubric, including how scores are totaled and how feedback will be delivered. Make sure the explanation is aligned with the needs of a "Teaching Assistant".

->>>>

We have details on scoring and instructions on how to use this rubric:

Scoring and Usage Instructions: 
{{step_6}}

Now, incorporate a section emphasizing the importance of academic integrity and ethical conduct, especially relevant to the grading process for {{course_name}}.

->>>>

We have scoring instructions for our rubric and a section on academic integrity:

Scoring and Usage Instructions: 
{{step_6}}

Academic Integrity and Ethics Section:
{{step_7}}

Also, allocate a section for overall comments and feedback, to give the "Teaching Assistant" a space to provide personalized insights to improve the student's future performance in {{course_name}}.

->>>>

We now added a section for overall feedback to our rubric:

Academic Integrity and Ethics Section:
{{step_7}}

Feedback Section:
{{step_8}}

Finally, summarize how the rubric aligns with the overall educational goals of the course or program: {{course_name}}. This will highlight the rubric's relevance to not just grading but also learning progress.


```

