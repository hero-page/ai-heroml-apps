# Board Game Review AI Composer

Explore the world of board games with Board Game Review AI Composer! Dive into AI-powered analyses of your favorite games. Specify your review variables for engaging, customized content that provides comprehensive game details, mechanics, aesthetics, and comparisons. From game setup to objective and personal verdicts - enjoy balanced, reliable, and entertaining reviews that bring unique, insightful perspectives to your board game experience.

To run this app online: [Board Game Review AI Composer Online](https://hero.page/app/board-game-review-ai-composer-comprehensive-ai-powered-board-game-analysis/jSZ6oOiqMoaNOEsCVUyz)

[![Run Board Game Review AI Composer Online](/assets/run.svg)](https://hero.page/app/board-game-review-ai-composer-comprehensive-ai-powered-board-game-analysis/jSZ6oOiqMoaNOEsCVUyz)

To learn more about AI Apps for Board Game Blogger use-cases in the Board Games & Tabletop RPGs industry, read [How to Elevate Board Game Blogs with AI-Powered Tools](https://hero.page/blog/ai/board-games-and-tabletop-rpgs/how-to-elevate-board-game-blogs-with-ai-powered-tools/170759)

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
npx hero run ./board_game_review_ai_composer.heroml
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
hero run ./board_game_review_ai_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./board_game_review_ai_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./board_game_review_ai_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./board_game_review_ai_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Board Game Review AI Composer
```
Your task is to write a game review for the Board Games & Tabletop RPGs industry, specifically for a board game blogger. We'll start with an introduction to entice the reader about the game, {{game_name}}.

Here's some more context about the Game Review:
Game Name: {{game_name}}

->>>>

Now we have a captivating introduction for our board game review:

Introduction:
{{step_1}}

Next, we will provide basic information about {{game_name}}, such as the designer, publisher, number of players, game duration, and difficulty level.

->>>>

Basic information about {{game_name}} is provided:

Introduction:
{{step_1}}

Game Information:
{{step_2}}

Now, let's create a section that elaborates on the game components and setup, depicting the quality of game pieces, ease of setup, and space requirement.

->>>>

We now have a description of the game components and setup:

Game Information:
{{step_2}}

Game Components and Setup:
{{step_3}}

Next, we need to provide a summary of the gameplay. The focus will not be on step-by-step rules, but rather on giving an impression of the flow and dynamism of {{game_name}}.

->>>>

We now have a brief summary of the gameplay:

Game Components and Setup:
{{step_3}}

Gameplay Summary:
{{step_4}}

Following this, analyze the game mechanics and the core elements of gameplay of {{game_name}}, discussing strategies, balancing, player interaction, randomness, and replayability.

->>>>

We have now analyzed the game mechanics of {{game_name}}:

Gameplay Summary:
{{step_4}}

Game Mechanics Analysis:
{{step_5}}

Let's now incorporate a section on 'Gameplay Highlights', where we focus on memorable moments, clever maneuvers, or engaging situations encountered while playing {{game_name}}.

->>>>

We now have a section focusing on gameplay highlights:

Game Mechanics Analysis:
{{step_5}}

Gameplay Highlights:
{{step_6}}

Next, assess the visual aesthetics and theme of {{game_name}}, addressing the artistic appeal, the coherence of design with the game's theme, and how well the theme is integrated into the gameplay.

->>>>

We have now assessed the visual aesthetics and theme of {{game_name}}:

Gameplay Highlights:
{{step_6}}

Visual Aesthetics and Theme Assessment:
{{step_7}}

Moving on, we'll discuss comparable games to {{game_name}}, indicating how they are similar or different, and recommending {{game_name}} for the fans of these games.

->>>>

Here are comparable games to {{game_name}}:

Visual Aesthetics and Theme Assessment:
{{step_7}}

Comparable Games:
{{step_8}}

Next, provide a clear evaluation and rating of {{game_name}}, taking into consideration all the aspects of the game we have discussed.

->>>>

Our evaluation and rating of {{game_name}} is here:

Comparable Games:
{{step_8}}

Game Evaluation and Rating:
{{step_9}}

Finally, lets include a 'Verdict' section that summarizes your key observations and provides a final recommendation, addressing if {{game_name}} is worth adding to a reader's game collection. 


```

