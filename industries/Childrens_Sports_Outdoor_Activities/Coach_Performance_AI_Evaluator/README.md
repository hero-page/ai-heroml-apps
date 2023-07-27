# Coach Performance AI Evaluator

Coach Performance AI Evaluator is a specialized youth sports coach evaluation tool with a difference. You can modify variables and prompts to make the tool highly personalized. It uses AI to analyze and produce high-quality comprehensive feedback covering areas like sports instruction, child development strategies, communication and team building skills. The unique attribute of the tool is the evaluation of not just the coach but also the progress of the children under their training. The final report holistically highlights coach's strengths, areas to improve, and expected growth trajectory.

To run this app online: [Coach Performance AI Evaluator Online](https://hero.page/app/coach-performance-ai-evaluator-customized-youth-sports-coach-evaluation/yrsr92WHcDIPtMxlJ91Y)

[![Run Coach Performance AI Evaluator Online](/assets/run.svg)](https://hero.page/app/coach-performance-ai-evaluator-customized-youth-sports-coach-evaluation/yrsr92WHcDIPtMxlJ91Y)

To learn more about AI Apps for Sports Coach use-cases in the Children's Sports & Outdoor Activities industry, read [How to Enhance Children's Sports Coaching with AI Tools](https://hero.page/blog/ai/children's-sports-and-outdoor-activities/how-to-enhance-children's-sports-coaching-with-ai-tools/170786)

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
npx hero run ./coach_performance_ai_evaluator.heroml
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
hero run ./coach_performance_ai_evaluator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./coach_performance_ai_evaluator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./coach_performance_ai_evaluator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./coach_performance_ai_evaluator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Coach Performance AI Evaluator
```
Your task is to write a "Performance Feedback" for the "Children's Sports & Outdoor Activities" industry, specifically for a "Sports Coach". 
Let's start with an introduction, where we briefly discuss the general performance of the coach throughout the evaluation period, as this will set the context for detailed feedback.

Here's some more context about the Performance Feedback:
General Performance: {{general_performance}}
Sports Instruction Skill: {{sports_instruction_skill}}
Motivation Inspiration Skill: {{motivation_inspiration_skill}}
Communication Skill: {{communication_skill}}
Discipline Management Skill: {{discipline_management_skill}}
Game Strategies Skill: {{game_strategies_skill}}
Team Building Skill: {{team_building_skill}}
Children Progression: {{children_progression}}
Child Friendly Methods Safety: {{child_friendly_methods_safety}}
Active Play Child Development: {{active_play_child_development}}
Conclusion: {{conclusion}}

->>>>

We have the introduction for our feedback on the sports coach, which provides a general assessment of their performance:

Introduction:
{{step_1}}

Next, discuss the competencies of the coach. We will touch on their skills in sports instruction, motivation and inspiration, communication, and discipline management.

->>>>

After discussing competencies, we now have more specific information on the coach's performance:

Introduction:
{{step_1}}

Competencies:
{{step_2}}

Next, let's determine and detail the coach's game strategies, specifically in terms of how they incorporate beneficial strategies into children's outdoor activities.

->>>>

So far, we've evaluated the sports coach's general performance, competencies, and game strategies:

Introduction:
{{step_1}}

Competencies:
{{step_2}}

Game Strategies:
{{step_3}}

Now, let's assess the coach's team building skills, particularly their ability to foster cooperation and strong relationships among the children.

->>>>

With the added assessment of team building skills, we now have:

Introduction:
{{step_1}}

Competencies:
{{step_2}}

Game Strategies:
{{step_3}}

Team Building Skills:
{{step_4}}

For the next step, we will look at the progression of the children's sports skills. We need to evaluate if their improvements or lack thereof can be attributed to the coach's techniques and methods.

->>>>

We have discussed the sports coach's general performance, competencies, game strategies, team building skills, and the progression of the children's skills:

Introduction:
{{step_1}}

Competencies:
{{step_2}}

Game Strategies:
{{step_3}}

Team Building Skills:
{{step_4}}

Children's Progression:
{{step_5}}

Next, we will provide feedback specific to the "Children's Sports & Outdoor Activities" industry. Details on the coach's adherence to child-friendly teaching methods, safety precautions, active play facilitation, and support for childhood development and health should be included.

->>>>

We have discussed the sports coach's general performance, competencies, game strategies, team building skills, children's progression, and industry-specific skills:

Introduction:
{{step_1}}

Competencies:
{{step_2}}

Game Strategies:
{{step_3}}

Team Building Skills:
{{step_4}}

Children's Progression:
{{step_5}}

Industry-Specific Skills:
{{step_6}}

Lastly, let's write a conclusion to summarize their overall performance, commend strengths, suggest possible areas for improvement, and express hopes for future enhancements.


```

