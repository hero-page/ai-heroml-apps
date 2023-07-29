# Hardware Release Notes Composer

The Hardware Release Notes Composer, an AI-Powered Hardware Release Summaries producing application, offers unmatched specificity and quality of content. Users can enter variable prompts, and the AI generates a detailed, customized summary of hardware product releases. Covering product updates, features, fixes, known issues, compatibility changes, upgrade instructions, support references, and legal disclaimers; it enlightens product managers with comprehensive knowledge about the latest product version. Renowned for its in-depth and tech-savvy content, it targets and caters to the needs of a professional audience. The harmony of high detail level and audience specificity is its unique attribute.

To run this app online: [Hardware Release Notes Composer Online](https://hero.page/app/hardware-release-notes-composer-ai-powered-hardware-release-summaries/Ygj33rP3TzYum6uzTMgj)

[![Run Hardware Release Notes Composer Online](/assets/run.svg)](https://hero.page/app/hardware-release-notes-composer-ai-powered-hardware-release-summaries/Ygj33rP3TzYum6uzTMgj)

To learn more about AI Apps for Product Manager use-cases in the Hardware Documentation industry, read [How to Streamline Hardware Documentation with AI Apps](https://hero.page/blog/ai/hardware-documentation/how-to-streamline-hardware-documentation-with-ai-apps/170935)

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
npx hero run ./hardware_release_notes_composer.heroml
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
hero run ./hardware_release_notes_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./hardware_release_notes_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./hardware_release_notes_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./hardware_release_notes_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

