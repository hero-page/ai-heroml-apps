# Environmental Impact AI Assessor

The Environmental Impact AI Assessor app provides an AI-powered platform for your project's comprehensive environmental assessment. The app allows users to specify variables in prompts to generate a customized, high-quality analysis. It delivers a detailed overview of a project’s potential environmental impacts and risks. Users enjoy information on baseline conditions, any negative impacts, and evaluation strategies. This includes mitigation measures, monitoring plans, stakeholder dialogues, and project alternatives. The app distinctively highlights the role of the Environmental Officer in reducing environment damage, and their engagement in risk mitigation, monitoring, and consultations.

To run this app online: [Environmental Impact AI Assessor Online](https://hero.page/app/environmental-impact-ai-assessor-ai-powered-project-environmental-assessment/AgvFOSPOondkodr0wBT0)

[![Run Environmental Impact AI Assessor Online](/assets/run.svg)](https://hero.page/app/environmental-impact-ai-assessor-ai-powered-project-environmental-assessment/AgvFOSPOondkodr0wBT0)

To learn more about AI Apps for Environmental Officer use-cases in the Environmental and Natural Resources Administration industry, read [How to Enhance Environmental Management with AI Tools](https://hero.page/blog/ai/environmental-and-natural-resources-administration/how-to-enhance-environmental-management-with-ai-tools/170858)

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
npx hero run ./environmental_impact_ai_assessor.heroml
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
hero run ./environmental_impact_ai_assessor.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./environmental_impact_ai_assessor.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./environmental_impact_ai_assessor.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./environmental_impact_ai_assessor.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

