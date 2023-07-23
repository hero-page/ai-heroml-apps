# Interactive Tutorial Plan Creator

Explore the power of AI with Interactive Tutorial Plan Creator, a one-stop app for creating personalized and comprehensive study guides. Boost learning outcomes with its unique feature of suggesting interactive doubt-clearing sessions. Generate a robust plan that combines clear learning objectives, a logically structured curriculum, engaging elements, key takeaways, tutorial summaries, and student feedback mechanisms. This student-centric app is designed to transform TAs into effective facilitators in academic and university settings.

To run this app online: [Interactive Tutorial Plan Creator Online](https://hero.page/app/interactive-tutorial-plan-creator-personalized-doubt-clearing-tutorial-design/biGQhQFvjjNrht43xsem)

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
npx hero run ./interactive_tutorial_plan_creator.heroml
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
hero run ./interactive_tutorial_plan_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./interactive_tutorial_plan_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./interactive_tutorial_plan_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./interactive_tutorial_plan_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Interactive Tutorial Plan Creator
```
Your task is to write a "Tutorial Plan" for the "Academic & University" industry, specifically for a "Teaching Assistant". 

Let's start with an introduction that defines the learning objectives for the tutorial. Provide an overview of what the students should achieve by the end of the tutorial and mention the learning objectives. 

Here's some more context about the Tutorial Plan:
Learning Objectives: {{learning_objectives}}
Curriculum Content: {{curriculum_content}}
Active Learning Elements: {{active_learning_elements}}
Key Points Takeaways: {{key_points_takeaways}}
Doubt Clearing Session: {{doubt_clearing_session}}

->>>>

Your "Tutorial Plan" commences with an overview and learning objectives:

Overview and Learning Objectives:
{{step_1}}

Now, outline the content to be covered in this tutorial based on the curriculum requirements. This content will serve as the main body of the tutorial. Also, ensure it is accurate, detailed, and comprehensive.

->>>>

The "Tutorial Plan" now has learning objectives and a comprehensive outline of the required content:

Learning Objectives:
{{step_1}}

Outline of Curriculum Content:
{{step_2}}

Next, structure this content in a logical, coherent manner. Group related concepts together and ensure that there is a natural progression from one topic to the next.

->>>>

Your "Tutorial Plan" displays its learning objectives and a well-structured outline of the curriculum content:

Learning Objectives:
{{step_1}}

Structured Curriculum Content:
{{step_3}}

Now, introduce active learning elements to the tutorial for a conversational and student-friendly experience. For instance, incorporate elements like question-and-answer segments, brief interactive activities, or prompts for group discussions.

->>>>

Your plan includes learning objectives, structured content, and active learning elements now:

Learning Objectives:
{{step_1}}

Structured Curriculum Content:
{{step_3}}

Active Learning Elements:
{{step_4}}

Next, highlight the key points and takeaways in each section of the tutorial. These points will assist the students in understanding, retaining, and reviewing essential concepts.

->>>>

The "Tutorial Plan" now includes learning objectives, structured content, active learning elements, and highlighted key points:

Learning Objectives:
{{step_1}}

Structured Curriculum Content:
{{step_3}}

Active Learning Elements:
{{step_4}}

Highlights and Key Takeaways:
{{step_5}}

Moving on, allocate some time towards the end for a doubt clearing session. This will allow TAs to handle the students' questions or direct them appropriately.

->>>>

With the addition of a time for a doubt clearing session, the "Tutorial Plan" now includes the following elements:

Learning Objectives:
{{step_1}}

Structured Curriculum Content:
{{step_3}}

Active Learning Elements:
{{step_4}}

Highlights and Key Takeaways:
{{step_5}}

Doubt Clearing Session:
{{step_6}}

Then, as a wrap-up, provide a succinct summary of the entire tutorial plan. This should involve reinstating the learning objectives and a brief overview of the key points.

->>>>

The summarized "Tutorial Plan" includes:

Learning Objectives:
{{step_1}}

Structured Curriculum Content:
{{step_3}}

Active Learning Elements:
{{step_4}}

Highlights and Key Takeaways:
{{step_5}}

Doubt Clearing Session:
{{step_6}}

Tutorial Summary:
{{step_7}}

Finally, incorporate a feedback mechanism for students to share their thoughts, suggestions, or concerns about the tutorial. This feedback mechanism will facilitate continuous improvement of the tutorial plan.


```

