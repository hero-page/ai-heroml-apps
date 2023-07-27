# Board Game Design Diary AI

Board Game Design Diary AI, an AI-Powered Board Game Creation Diary, generates comprehensive insights about a designer's design process. Detailing the game's concept, brainstorming, research, development of game mechanics, playtesting for balance, iterations, design refinements, and summarizing the entire production process, the app provides an in-depth, industry-specific narrative. It emphasizes the overcome challenges, pivotal decisions, usage of relevant terminology, and learnings for future game designs. Expect an extensive examination into the board games and tabletop RPG design process.

To run this app online: [Board Game Design Diary AI Online](https://hero.page/app/board-game-design-diary-ai-ai-powered-board-game-creation-diary/Zx8vUXkaEhQIMEbZk2Ts)

[![Run Board Game Design Diary AI Online](/assets/run.svg)](https://hero.page/app/board-game-design-diary-ai-ai-powered-board-game-creation-diary/Zx8vUXkaEhQIMEbZk2Ts)

To learn more about AI Apps for Game Designer use-cases in the Board Games & Tabletop RPGs industry, read [How to Elevate Board Game Design with AI Analysis and Review](https://hero.page/blog/ai/board-games-and-tabletop-rpgs/how-to-elevate-board-game-design-with-ai-analysis-and-review/170757)

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
npx hero run ./board_game_design_diary_ai.heroml
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
hero run ./board_game_design_diary_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./board_game_design_diary_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./board_game_design_diary_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./board_game_design_diary_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Board Game Design Diary AI
```
Your task is to write a "Design Process Diary" for the "Board Games & Tabletop RPGs" industry, specifically for a "Game Designer". Let's start with an introduction which will explain the purpose of the "Design Process Diary": {{design_goal}}.

Here's some more context about the Design Process Diary:
Design Goal: {{design_goal}}
Game Concept: {{game_concept}}
Game Mechanics: {{game_mechanics}}
Playtesting Insights: {{playtesting_insights}}
Design Iterations: {{design_iterations}}
Future Design Projects: {{future_design_projects}}

->>>>

The purpose of our "Design Process Diary" is:

Purpose:
{{step_1}}

Let's use this as a basis to describe the game concept: {{game_concept}}.

->>>>

With the defined purpose, we can now move forward:

Purpose:
{{step_1}}

Our concept for the game:

Game Concept:
{{step_2}}

Next, let's create a game concept development section. We will detail the brainstorming and research process that led to the creation of the game idea: {{game_concept}}.

->>>>

Our journey so far:

Purpose:
{{step_1}}

Game Concept:
{{step_2}}

Brainstorming and Research Process:
{{step_3}}

Now, include a game mechanics development section. This section will discuss the different mechanics that were considered, discarded, and included in the game design: {{game_mechanics}}.

->>>>

This is what we've achieved so far:

Brainstorming and Research Process:
{{step_3}}

Game Mechanics Development:
{{step_4}}

Next, let's create a game balance and playtesting section. This section will highlight the efforts made to ensure the game is balanced and enjoyable, and also provide insights obtained from playtesting: {{playtesting_insights}}.

->>>>

So far, we have these entries in our design process diary:

Game Mechanics Development:
{{step_4}}

Game Balance and Playtesting:
{{step_5}}

Next, include an iteration and refinement section. This section will detail the changes made through various iterations: {{design_iterations}}, and how you refined the game based on playtesting and feedback.

->>>>

Following is what we have in our diary:

Game Balance and Playtesting:
{{step_5}}

Iteration and Refinement:
{{step_6}}

Finally, let's create a conclusion section recapturing the core elements of the journey in turning the concept {{game_concept}} into a well-rounded and enjoyable game and summarizing the development and design process: {{design_goal}}.

->>>>

We're almost finished:

Iteration and Refinement:
{{step_6}}

Conclusion:
{{step_7}}

We should inject industry-specific language throughout the diary to lend credibility and professionalism. Draft a revision of each section, ensuring to describe mechanics, theme, components, player interaction and game dynamics with industry terms.

->>>>

So far, we've added industry-specific language to our diary:

Professional Diary:
{{step_8}}

Next, re-iterate throughout the diary, including the challenges faced at every step and how they were overcome to provide a comprehensive process diary.

->>>>

Following is our updated diary with information about all challenges:

Updated & Comprehensive Diary:
{{step_9}}

Let's revise our diary yet again treating it as a narrative of our creative journey, highlighting important design decisions, breakthroughs, and turning points in the development process.

->>>>

Here's our narrative diary:

Narrative Diary:
{{step_10}}

Lastly, conclude the diary with reflections on the lessons learned from the process and how these insights could be applied to future design projects: {{future_design_projects}}.


```

