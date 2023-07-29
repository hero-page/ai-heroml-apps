# School Recycling Plan Creator

With the School Recycling Plan Creator, you can craft ultra-tailored strategies for a greener campus. Powered by advanced AI, this app generates robust content on school recycling, illustrating its importance, objectives, methodology, and benefits. Interacting with its prompts allows personalisation of the plan, detailing waste management, target audience, and planning strategies. Beyond providing general advice, it specifically tackles procedures for different waste types, like paper, plastic, food or e-waste. Incorporating real-life examples and potential partnerships, it's your route to a fully sustainable school environment.

To run this app online: [School Recycling Plan Creator Online](https://hero.page/app/school-recycling-plan-creator-customized-school-recycling-strategies/kSgCaAW7IoVsEDUaEz2O)

[![Run School Recycling Plan Creator Online](/assets/run.svg)](https://hero.page/app/school-recycling-plan-creator-customized-school-recycling-strategies/kSgCaAW7IoVsEDUaEz2O)

To learn more about AI Apps for Eco Club Member use-cases in the High School Students - Environmental Sciences industry, read [How to Elevate Eco Club Initiatives With AI for Environmental Science](https://hero.page/blog/ai/high-school-students-environmental-sciences/how-to-elevate-eco-club-initiatives-with-ai-for-environmental-science/170953)

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
npx hero run ./school_recycling_plan_creator.heroml
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
hero run ./school_recycling_plan_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./school_recycling_plan_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./school_recycling_plan_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./school_recycling_plan_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

