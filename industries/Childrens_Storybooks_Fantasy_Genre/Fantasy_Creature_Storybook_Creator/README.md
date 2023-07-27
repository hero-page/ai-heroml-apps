# Fantasy Creature Storybook Creator

Dive into an enchanting world with Fantasy Creature Storybook Creator. This app employs advanced AI technology to fabricate high-quality, customized storybook adventures where you can define a magical creature's name, origin, abilities and role. These beguiling descriptions are infused with educational morals, kept captivatingly consistent to maintain child engagement, and fuses the character traits with the existing fantasy realm rules, creating an immersive and constructive reading experience for kids.

To run this app online: [Fantasy Creature Storybook Creator Online](https://hero.page/app/fantasy-creature-storybook-creator-customize-magical-creatures'-storybook-adventure/TVwtnPqSZC9Mg1G9h305)

[![Run Fantasy Creature Storybook Creator Online](/assets/run.svg)](https://hero.page/app/fantasy-creature-storybook-creator-customize-magical-creatures'-storybook-adventure/TVwtnPqSZC9Mg1G9h305)

To learn more about AI Apps for Author use-cases in the Children's Storybooks - Fantasy Genre industry, read [How to Amplify Kids' Fantasy Story Writing with AI Tools](https://hero.page/blog/ai/children's-storybooks-fantasy-genre/how-to-amplify-kids'-fantasy-story-writing-with-ai-tools/170798)

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
npx hero run ./fantasy_creature_storybook_creator.heroml
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
hero run ./fantasy_creature_storybook_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./fantasy_creature_storybook_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./fantasy_creature_storybook_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./fantasy_creature_storybook_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

