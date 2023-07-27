# Educational Storybook Review Generator

Explore the power of AI with the Educational Storybook Review Generator. This unique app allows users to provide customized prompts, which the app's AI interprets to create comprehensive, detailed reviews of a children's educational storybook. Each review weighs the book's age-appropriateness, curriculum relevance, themes, pace, structure, creativity, interactivity, content accuracy, and educational standards alignment to provide a thorough assessment. Offering beneficial pointers for improvement, this app focuses on enriching the educational value of children's storybooks.

To run this app online: [Educational Storybook Review Generator Online](https://hero.page/app/educational-storybook-review-generator-ai-powered-educational-book-assessment/V4iMsc0ORV3uEkeDY0Yw)

[![Run Educational Storybook Review Generator Online](/assets/run.svg)](https://hero.page/app/educational-storybook-review-generator-ai-powered-educational-book-assessment/V4iMsc0ORV3uEkeDY0Yw)

To learn more about AI Apps for Educational Consultant use-cases in the Children's Storybooks - Educational Books industry, read [How to Enhance Storybook Education with AI-Driven Learning Objectives and Lesson Plans](https://hero.page/blog/ai/children's-storybooks-educational-books/how-to-enhance-storybook-education-with-ai-driven-learning-objectives-and-lesson-plans/170797)

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
npx hero run ./educational_storybook_review_generator.heroml
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
hero run ./educational_storybook_review_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./educational_storybook_review_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./educational_storybook_review_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./educational_storybook_review_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

