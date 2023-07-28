# Wellness Retreat Review Generator

Wellness Retreat Review Generator, your personalized eco-wellness retreat review platform. The app leverages AI to create customized, high-quality reviews from the standpoint of a wellness blogger. Specify variables to curate a comprehensive critique focusing on retreat location, facilities, staff, activities, personal experiences and more. Unique attribute of the content includes a subjective view of retreats in Ecotherapy & Nature Connection, emphasizing the holistic impact on wellbeing and sustainability. This makes the app perfect for wellness and nature enthusiasts.

To run this app online: [Wellness Retreat Review Generator Online](https://hero.page/app/wellness-retreat-review-generator-personalized-eco-wellness-retreat-reviews/sRuKGtOM2HcGopCoizXl)

[![Run Wellness Retreat Review Generator Online](/assets/run.svg)](https://hero.page/app/wellness-retreat-review-generator-personalized-eco-wellness-retreat-reviews/sRuKGtOM2HcGopCoizXl)

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
npx hero run ./wellness_retreat_review_generator.heroml
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
hero run ./wellness_retreat_review_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./wellness_retreat_review_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./wellness_retreat_review_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./wellness_retreat_review_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

