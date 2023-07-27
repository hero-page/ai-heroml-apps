# Young Readers StoryCraft AI

Young Readers StoryCraft AI is a dynamic app that uses machine learning to generate compelling narratives for young readers. It allows users to input specific variables like main characters, conflicts, and more, crafting an intricate plot that covers all essential parts of a story. Unique to this app is the emphasis on 'teachable moments', educational tidbits embedded within the story to enlighten young minds. Plus, its narratives always offer a realistic, relatable resolution, ensuring each story resonates with its young audience. Designed with the Children's Storybooks - Young Adult Novels industry in mind, it ensures age-appropriate content.

To run this app online: [Young Readers StoryCraft AI Online](https://hero.page/app/young-readers-storycraft-ai-ai-narrative-craft-for-young-readers/iS4nuFjBFVE9popfmByz)

[![Run Young Readers StoryCraft AI Online](/assets/run.svg)](https://hero.page/app/young-readers-storycraft-ai-ai-narrative-craft-for-young-readers/iS4nuFjBFVE9popfmByz)

To learn more about AI Apps for Author use-cases in the Children's Storybooks - Young Adult Novels industry, read [How to Enhance YA Novel Writing with AI-Driven Character Development](https://hero.page/blog/ai/children's-storybooks-young-adult-novels/how-to-enhance-ya-novel-writing-with-ai-driven-character-development/170804)

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
npx hero run ./young_readers_storycraft_ai.heroml
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
hero run ./young_readers_storycraft_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./young_readers_storycraft_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./young_readers_storycraft_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./young_readers_storycraft_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

