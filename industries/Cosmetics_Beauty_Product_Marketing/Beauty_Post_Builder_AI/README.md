# Beauty Post Builder AI

The Beauty Post Builder AI, with a core focus on AI-driven beauty marketing content creation, enables users to shape variables in prompts for custom content. It leverages AI to craft premium, personalized posts promoting cosmetics and beauty products. The distinctive feature lies in its strategic creation of engaging content aligning with current beauty trends and influencer endorsements. Perfect for detailed introductions, showcasing unique selling points, usage rates, origin, availability, pricing, and promotional offers. It's your innovative companion for powerful, trend-driven beauty marketing.

To run this app online: [Beauty Post Builder AI Online](https://hero.page/app/beauty-post-builder-ai-ai-driven-beauty-marketing-content/TufL3hhqGWFET9Buxf3G)

[![Run Beauty Post Builder AI Online](/assets/run.svg)](https://hero.page/app/beauty-post-builder-ai-ai-driven-beauty-marketing-content/TufL3hhqGWFET9Buxf3G)

To learn more about AI Apps for Content Creator use-cases in the Cosmetics & Beauty Product Marketing industry, read [How to Elevate Beauty Content Creation with AI in Makeup Tutorials, Social Media, and Product Reviews](https://hero.page/blog/ai/cosmetics-and-beauty-product-marketing/how-to-elevate-beauty-content-creation-with-ai-in-makeup-tutorials-social-media-and-product-reviews/170822)

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
npx hero run ./beauty_post_builder_ai.heroml
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
hero run ./beauty_post_builder_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./beauty_post_builder_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./beauty_post_builder_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./beauty_post_builder_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

