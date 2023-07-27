# Board Game Mechanics Analyzer

The Board Game Mechanics Analyzer app uses advanced AI technology to offer a comprehensive review of game mechanics for board games and tabletop RPGs. Define certain variables and get a detailed overview covering a game's title, objective, mechanics, unique attributes, player interaction, progression, and required skills. The result is an in-depth analysis, incorporating industry-specific terms for enhanced understanding. This tool offers a unique perspective on games that goes beyond standard rulebooks or reviews.

To run this app online: [Board Game Mechanics Analyzer Online](https://hero.page/app/board-game-mechanics-analyzer-comprehensive-analysis-of-game-mechanics/hQWMyAwV4RJg2YryINge)

[![Run Board Game Mechanics Analyzer Online](/assets/run.svg)](https://hero.page/app/board-game-mechanics-analyzer-comprehensive-analysis-of-game-mechanics/hQWMyAwV4RJg2YryINge)

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
npx hero run ./board_game_mechanics_analyzer.heroml
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
hero run ./board_game_mechanics_analyzer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./board_game_mechanics_analyzer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./board_game_mechanics_analyzer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./board_game_mechanics_analyzer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Board Game Mechanics Analyzer
```
Your task is to write a "Game Mechanics Description" for the "Board Games & Tabletop RPGs" industry, specifically for a "Game Designer". Let's start by introducing the game title and providing some brief background or context to the game: {{game_title}} and {{game_background}}. This background should include what type of game it is, its thematic elements, and its inspiration.

Here's some more context about the Game Mechanics Description:
Game Title: {{game_title}}
Game Background: {{game_background}}
Game Objective: {{game_objective}}
Basic Mechanics: {{basic_mechanics}}
Unique Mechanics: {{unique_mechanics}}
Player Interaction: {{player_interaction}}
Game Progression: {{game_progression}}
Game Skill Requirements: {{game_skill_requirements}}
Game Summary: {{game_summary}}

->>>>

Now that we have our title and game background:

Game Title:
{{step_1}}

Game Background:
{{step_2}}

Next, let's focus on presenting the principal objective of the game. This should provide a high-level understanding of the game's end goal, how players can win or lose, and what are the key driving elements of the gameplay.

->>>>

With the game objective in place:

Game Objective:
{{step_3}}

Let's move on to describing the basic game mechanics. This step should involve information on how a player interacts with the game, such as moving, attacking, scoring points, etc. The mechanics should demonstrate how those actions are done, what tools or resources players need, and the outcomes of those actions.

->>>>

Next, we have a grasp on the basic game mechanics:

Basic Game Mechanics:
{{step_4}}

Now let's detail the game's unique mechanics or features that set it apart. This step should focus on those elements that elevate the game above its competitors or make it distinctive in the market.

->>>>

We now have a clear understanding of the game's unique mechanics or features:

Unique Game Mechanics:
{{step_5}}

After that, let's move on to describing player interaction in the game. This step involves discussing how players interact with game elements, in-game characters, other players, and the game environment. This description should explore both cooperative and competitive elements, as well as any single-player components.

->>>>

Now that we have described player interaction:

Player Interaction:
{{step_6}}

We should move on to explaining the game's progression. This includes how the game rounds or turns are structured, how the game progresses towards its end, and defining situations that generate changes or disrupt the game flow.

->>>>

Having defined the game's progression:

Game Progression:
{{step_7}}

We should now describe the game's skill requirements. This should touch on what skills or strategies players need to excel in the game, like strategic planning, bluffing, team collaboration, or quick reflexes.


```

