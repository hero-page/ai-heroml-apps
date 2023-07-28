# Ecotherapy Journey Content Creator

Explore the healing wilderness with Ecotherapy Journey Content Creator. Uniquely blend personal narratives with industry insights using customizable AI suggestions. Personalize prompts to share transformative experiences, breakthroughs, and connect with ecotherapy. Enrich your wellness blog, not just as a personal anecdote but as an intriguing, holistic perspective on ecotherapy industry. Navigate your journey and engage readers in a meaningful way.

To run this app online: [Ecotherapy Journey Content Creator Online](https://hero.page/app/ecotherapy-journey-content-creator-personalized-ecotherapy-journey-insights/wFQX296bAWa9FLZGP9wq)

[![Run Ecotherapy Journey Content Creator Online](/assets/run.svg)](https://hero.page/app/ecotherapy-journey-content-creator-personalized-ecotherapy-journey-insights/wFQX296bAWa9FLZGP9wq)

To learn more about AI Apps for Wellness Blogger use-cases in the Ecotherapy & Nature Connection industry, read [How to Elevate Your Wellness Blog with AI-Enhanced Ecotherapy Content](https://hero.page/blog/ai/ecotherapy-and-nature-connection/how-to-elevate-your-wellness-blog-with-ai-enhanced-ecotherapy-content/170851)

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
npx hero run ./ecotherapy_journey_content_creator.heroml
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
hero run ./ecotherapy_journey_content_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ecotherapy_journey_content_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ecotherapy_journey_content_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ecotherapy_journey_content_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

