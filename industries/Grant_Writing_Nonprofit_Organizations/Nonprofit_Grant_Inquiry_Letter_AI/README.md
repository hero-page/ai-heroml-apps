# Nonprofit Grant Inquiry Letter AI

Harness the power of AI with the Nonprofit Grant Inquiry Letter AI app. Define your variables and let the AI create bespoke, high-quality content that speaks volumes about your organization and its mission. The auto-generated, professional-grade Letter of Inquiry streamlines your nonprofit's grant application process. With rich details about your project, its implementation strategy, the problems it aims to solve, expected outcomes, and a budget estimate, our AI-written letters excel in appealing to potential funders' interests. Our unique touch? We make your noble cause resonate with your readers, fostering deeper connections to secure their support.

To run this app online: [Nonprofit Grant Inquiry Letter AI Online](https://hero.page/app/nonprofit-grant-inquiry-letter-ai-ai-crafted-nonprofit-grant-letters/XX2usApSsWEx9LPvbwAK)

[![Run Nonprofit Grant Inquiry Letter AI Online](/assets/run.svg)](https://hero.page/app/nonprofit-grant-inquiry-letter-ai-ai-crafted-nonprofit-grant-letters/XX2usApSsWEx9LPvbwAK)

To learn more about AI Apps for Grant Writer use-cases in the Grant Writing - Nonprofit Organizations industry, read [How to Create Winning Nonprofit Funding Proposals with AI Tools](https://hero.page/blog/ai/grant-writing-nonprofit-organizations/how-to-create-winning-nonprofit-funding-proposals-with-ai-tools/170923)

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
npx hero run ./nonprofit_grant_inquiry_letter_ai.heroml
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
hero run ./nonprofit_grant_inquiry_letter_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./nonprofit_grant_inquiry_letter_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./nonprofit_grant_inquiry_letter_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./nonprofit_grant_inquiry_letter_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

