# Ghostwriting Discussion Customizer

Explore the depth of the ghostwriting industry with Ghostwriting Discussion Customizer, an AI-powered analyst exclusively for the blogging sphere. Set your unique parameters to generate a tailored, high-quality conversation around particular industry trends, issues or problems. The app's prowess lies in crafting comprehensive dialogue, providing detailed background information, sharing insightful examples and anecdotes, presenting an acute analysis of your designated topic, and suggesting prospective solutions. Curated discussions around merits and drawbacks are enriched, ending with a powerful conclusion emphasizing the central theme or problem demanding wider conversations in the writing communities. With its intricate focus, the app is uniquely positioned, guiding you deeper than the generic surface.

To run this app online: [Ghostwriting Discussion Customizer Online](https://hero.page/app/ghostwriting-discussion-customizer-ai-powered-ghostwriting-industry-analyst/sSBJtfLluYX2jwfy1K0c)

[![Run Ghostwriting Discussion Customizer Online](/assets/run.svg)](https://hero.page/app/ghostwriting-discussion-customizer-ai-powered-ghostwriting-industry-analyst/sSBJtfLluYX2jwfy1K0c)

To learn more about AI Apps for Blogger use-cases in the Ghostwriting industry, read [How to Elevate Ghostwriting with AI-Driven Insights and Tips](https://hero.page/blog/ai/ghostwriting/how-to-elevate-ghostwriting-with-ai-driven-insights-and-tips/170902)

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
npx hero run ./ghostwriting_discussion_customizer.heroml
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
hero run ./ghostwriting_discussion_customizer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ghostwriting_discussion_customizer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ghostwriting_discussion_customizer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ghostwriting_discussion_customizer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```
