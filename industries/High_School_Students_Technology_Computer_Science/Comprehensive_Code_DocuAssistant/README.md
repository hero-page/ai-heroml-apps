# Comprehensive Code Docu-Assistant

Comprehensive Code Docu-Assistant makes understanding complex coding simple with AI-powered customization. Specify variables in prompts for a bespoke experience, leading to a thorough and articulate code documentation. Discover each line's functionality, code operation, logical flow and more in detail. The app's unique thoroughness ensures high readability, making it not only helpful to the code author but also for other students and interested folks. With an integral summary feature, code's original purpose is never lost in the details. Forge an enlightening journey into the world of coding.

To run this app online: [Comprehensive Code Docu-Assistant Online](https://hero.page/app/comprehensive-code-docu-assistant-smart-detailed-code-understanding/WEbpMz7VbY0XcwhoXHsX)

[![Run Comprehensive Code Docu-Assistant Online](/assets/run.svg)](https://hero.page/app/comprehensive-code-docu-assistant-smart-detailed-code-understanding/WEbpMz7VbY0XcwhoXHsX)

To learn more about AI Apps for Student use-cases in the High School Students - Technology & Computer Science industry, read [How to Excel in Tech Studies with AI-Assisted Code Documentation, Website Design Planning and Data Analysis](https://hero.page/blog/ai/high-school-students-technology-and-computer-science/how-to-excel-in-tech-studies-with-ai-assisted-code-documentation-website-design-planning-and-data-analysis/170973)

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
npx hero run ./comprehensive_code_docu_assistant.heroml
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
hero run ./comprehensive_code_docu_assistant.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./comprehensive_code_docu_assistant.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./comprehensive_code_docu_assistant.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./comprehensive_code_docu_assistant.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

