# Children's Storybook Setting & Education AI

Step into the delightful realm of stories with the Childrens Storybook Setting & Education AI. This unique app blends fun and learning, allowing you to personalize variables, resulting in tailor-made interactive tales. Harness the power of AI to get high-quality, thrilling content. Settings come alive, rich with details about time, location, and intriguing non-human characters. Stimulate your child's imagination while nurturing their curiosity. The crown jewel of this app is the perfect fusion of interactive storytelling with insightful educational facts pertinent to the story's theme. Dive deep into a story set in the sea and emerge with fascinating knowledge about marine life. An immersive reading experience that doubles as a learning toolkit. Create memorable moments with stories that come alive.

To run this app online: [Children's Storybook Setting & Education AI Online](https://hero.page/app/children's-storybook-setting-and-education-ai-interactive-learning-through-storytelling/oB3ghpLQ3eYNvcnLCo8X)

[![Run Children's Storybook Setting & Education AI Online](/assets/run.svg)](https://hero.page/app/children's-storybook-setting-and-education-ai-interactive-learning-through-storytelling/oB3ghpLQ3eYNvcnLCo8X)

To learn more about AI Apps for Author use-cases in the Children's Storybooks - Educational Books industry, read [How to Craft Enthralling Educational Storybooks Using AI Tools](https://hero.page/blog/ai/children's-storybooks-educational-books/how-to-craft-enthralling-educational-storybooks-using-ai-tools/170795)

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
npx hero run ./childrens_storybook_setting_and_education_ai.heroml
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
hero run ./childrens_storybook_setting_and_education_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./childrens_storybook_setting_and_education_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./childrens_storybook_setting_and_education_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./childrens_storybook_setting_and_education_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

