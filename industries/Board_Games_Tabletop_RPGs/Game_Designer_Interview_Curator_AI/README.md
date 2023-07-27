# Game Designer Interview Curator AI

Discover the 'Game Designer Interview Curator AI' app, offering detailed game designer interviews through AI technology. Customize prompts, exploring depths of designers' experience, process, methods, and their notable games. Gain insights into mechanic design, player interaction, theme incorporation, game development, and business aspects. Ideal for aspiring designers and gaming enthusiasts. Unique in-depth exploration offers unmatched industry insights.

To run this app online: [Game Designer Interview Curator AI Online](https://hero.page/app/game-designer-interview-curator-ai-insightful-ai-curated-game-design-interviews/fGTapi4EBef6DE1hguR1)

[![Run Game Designer Interview Curator AI Online](/assets/run.svg)](https://hero.page/app/game-designer-interview-curator-ai-insightful-ai-curated-game-design-interviews/fGTapi4EBef6DE1hguR1)

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
npx hero run ./game_designer_interview_curator_ai.heroml
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
hero run ./game_designer_interview_curator_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./game_designer_interview_curator_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./game_designer_interview_curator_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./game_designer_interview_curator_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Game Designer Interview Curator AI
```
Let's conduct an interview with a game designer for the Board Games & Tabletop RPGs industry, specifically targeted at a Board Game Blogger. The interview will start with a short introduction of the {{game_designer}} and their notable works, followed by discussions around their background, the game design process, specific games they've designed, tips and advice for future game designers, and finally wrapping up the interview with a conclusion. 

The first step is to draft a brief introduction for the {{game_designer}}, their notable games, and the purpose of this interview.

Here's some more context about the Interview with Game Designer:
Game Designer: {{game_designer}}
Specific Game: {{specific_game}}

->>>>

Now we have our introduction:

Introduction:
{{step_1}}

Now, discuss the experience, journey and credentials of this {{game_designer}} as they ventured into game design, building up to their current stature.

->>>>

Given the introduction:

Introduction:
{{step_1}}

This is the summarized background of our {{game_designer}}:

Background:
{{step_2}}

Next, we need to explore the {{game_designer}}'s game design process, their inspirations, ideologies, and the techniques they use.

->>>>

Having explored their background:

Background:
{{step_2}}

We now have in-depth insights into the {{game_designer}}'s game design process:

Game Design Process:
{{step_3}}

Now, let's discuss in detail about their more notable games or any {{specific_game}} chosen by the blogger. Focus must be on the creation process, challenges faced, and the final product.

->>>>

In addition to their game design process:

Game Design Process:
{{step_3}}

We have delved into the designer's well known games:

Specific Games Discussed:
{{step_4}}

Then, ask the {{game_designer}} to share some advice and tips for aspiring board game designers.

->>>>

Drawing from the insights into their notable games:

Specific Games Discussed:
{{step_4}}

The {{game_designer}} has provided these tips and advice for future game designers:

Tips and Advice:
{{step_5}}

Finally, we need to wrap up the interview by summarizing the main points, showcasing the journey we took from the introduction, through the designer's background, process, games, to their advice, and then, present a token of appreciation towards the {{game_designer}} for their time and contribution.


```

