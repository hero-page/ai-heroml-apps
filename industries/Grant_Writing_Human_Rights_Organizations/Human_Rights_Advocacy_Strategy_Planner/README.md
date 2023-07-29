# Human Rights Advocacy Strategy Planner

Human Rights Advocacy Strategy Planner is a strategic planning tool for human rights advocacy. This advanced app uses AI to generate customized, superior quality content for program directors in human rights organizations. Users can input specific variables prompting the app to create comprehensive strategic plans. These plans outline advocacy strategies, provide human rights context, define advocacy goals, identify stakeholders and detail advocacy tactics. Additionally, they explain resource allocation, evaluate the plan and schedule execution. With a unique focus on human rights, the app understands the dynamics of the field and offers guidance on influencing stakeholders. A patent testament to commitment to human rights.

To run this app online: [Human Rights Advocacy Strategy Planner Online](https://hero.page/app/human-rights-advocacy-strategy-planner-strategic-planning-for-human-rights-advocacy/Jzp9zrJC4D4WebAzhWeH)

[![Run Human Rights Advocacy Strategy Planner Online](/assets/run.svg)](https://hero.page/app/human-rights-advocacy-strategy-planner-strategic-planning-for-human-rights-advocacy/Jzp9zrJC4D4WebAzhWeH)

To learn more about AI Apps for Program Director use-cases in the Grant Writing - Human Rights Organizations industry, read [How to Elevate Grant Writing With AI in Human Rights Advocacy](https://hero.page/blog/ai/grant-writing-human-rights-organizations/how-to-elevate-grant-writing-with-ai-in-human-rights-advocacy/170920)

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
npx hero run ./human_rights_advocacy_strategy_planner.heroml
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
hero run ./human_rights_advocacy_strategy_planner.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./human_rights_advocacy_strategy_planner.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./human_rights_advocacy_strategy_planner.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./human_rights_advocacy_strategy_planner.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

