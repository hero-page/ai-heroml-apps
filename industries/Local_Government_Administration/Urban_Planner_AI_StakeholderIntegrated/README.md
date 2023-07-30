# Urban Planner AI: Stakeholder-Integrated

Experience an AI-enabled, seamless urban development planning with Urban Planner AI: Stakeholder-Integrated. It allows users to input specifics that guide high-quality content generation, covering detailed urban development plans from current state analysis to vision deployment. Uniquely, it incorporates strategies for stakeholder engagement and risk mitigation, ensuring a comprehensive, proactive and inclusive urban planning process. Its output includes implementation timelines, budget estimates, proposals for housing, commerce, and infrastructure improvements, making it an exhaustive tool for smart, all-inclusive urban planning.

To run this app online: [Urban Planner AI: Stakeholder-Integrated Online](https://hero.page/app/urban-planner-ai:-stakeholder-integrated-ai-powered-inclusive-urban-development/v7MaDq4AIJZFNwDPEcou)

[![Run Urban Planner AI: Stakeholder-Integrated Online](/assets/run.svg)](https://hero.page/app/urban-planner-ai:-stakeholder-integrated-ai-powered-inclusive-urban-development/v7MaDq4AIJZFNwDPEcou)

To learn more about AI Apps for City Planner use-cases in the Local Government Administration industry, read [How to Propel Urban Planning with AI-aided Tools](https://hero.page/blog/ai/local-government-administration/how-to-propel-urban-planning-with-ai-aided-tools/171020)

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
npx hero run ./urban_planner_ai_stakeholder_integrated.heroml
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
hero run ./urban_planner_ai_stakeholder_integrated.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./urban_planner_ai_stakeholder_integrated.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./urban_planner_ai_stakeholder_integrated.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./urban_planner_ai_stakeholder_integrated.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

