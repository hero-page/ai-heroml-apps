# Game Design Review AI Creator

Game Design Review AI Creator is your go-to for AI-powered analysis of game design. Input variables into prompts and let the AI do the rest by generating detailed, customized content. The app ensures a comprehensive game critique from a game designer’s view, covering aspects like aesthetics, gameplay mechanics, theme, and potential improvements. You will even receive insights on the game's relevance and influence within the Board Games & Tabletop RPGs industry. Expect a unique perspective that ordinary reviews may miss.

To run this app online: [Game Design Review AI Creator Online](https://hero.page/app/game-design-review-ai-creator-ai-powered-game-design-analysis/iDrZP1X1mhK941fX1U8e)

[![Run Game Design Review AI Creator Online](/assets/run.svg)](https://hero.page/app/game-design-review-ai-creator-ai-powered-game-design-analysis/iDrZP1X1mhK941fX1U8e)

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
npx hero run ./game_design_review_ai_creator.heroml
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
hero run ./game_design_review_ai_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./game_design_review_ai_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./game_design_review_ai_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./game_design_review_ai_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Game Design Review AI Creator
```
Write a game review for the Board Games & Tabletop RPGs industry, specifically for a Game Designer. Let's start with an engaging introduction about the game being reviewed.

Here's some more context about the Game Review:
Game Description: {{game_description}}
Game Design Details: {{game_design_details}}
Artwork And Theme: {{artwork_and_theme}}
Gameplay Mechanics: {{gameplay_mechanics}}
Game Originality: {{game_originality}}
Game Replayability: {{game_replayability}}
Improvement Suggestions: {{improvement_suggestions}}
Game Summary: {{game_summary}}

->>>>

This is the introduction for our game review:

Introduction:
{{step_1}}

Next, let's elaborate on the game's design, focusing on elements that would intrigue a Game Designer.

->>>>

So far, we have an introduction and details on the game's design:

Introduction:
{{step_1}}

Game's Design Details:
{{step_2}}

Now, we should delve into the artwork, theme, and aesthetics of the game, and how they influence the player's experience.

->>>>

At this point, we have information on the artwork, theme and aesthetics:

Introduction:
{{step_1}}

Game's Design Details:
{{step_2}}

Artwork and Theme:
{{step_3}}

Next, talk about the gameplay mechanics. Explain how the game's rules, player interactions, and system complexity operate.

->>>>

It's time to look at what we have on gameplay mechanics:

Introduction:
{{step_1}}

Game's Design Details:
{{step_2}}

Artwork and Theme:
{{step_3}}

Gameplay Mechanics:
{{step_4}}

Moving forward, let's analyze and discuss the game's originality. Compare it to other similar games in the industry and highlight what sets it apart.

->>>>

Now, let's see the game's originality:

Introduction:
{{step_1}}

Gameplay Mechanics:
{{step_4}}

Game Originality:
{{step_5}}

Next on our list is to evaluate the game's replayability. Comment on the variety, depth, and enjoyment found in repeated plays.

->>>>

Here's what we have about the game's replayability:

Introduction:
{{step_1}}

Game Originality:
{{step_5}}

Game Replayability:
{{step_6}}

To make this review beneficial for a Game Designer, let's highlight some ways to improve the game. Suggest tweaks that could enhance its appeal and gameplay.

->>>>

Now, let's look at the section that provides suggestions for improvement:

Introduction:
{{step_1}}

Game Replayability:
{{step_6}}

Improvement Suggestions:
{{step_7}}

For our final step, let's summarize the review. Highlight the game's primary merits and drawbacks along with its relevance and impact on the industry.


```

