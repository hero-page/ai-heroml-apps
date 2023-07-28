# EcoBrand Meeting Minutes Generator

EcoBrand Meeting Minutes Generator is a powerful AI-powered tool, engineered for Brand Managers in the Eco-friendly & Sustainable Product Marketing industry. Effortlessly input variables to yield customized, high-quality meeting records, including meeting details, attendee list, agenda overview, discussion summaries, and assigned tasks. Stay informed with latest industry trends, competitor strategies, and eco-product updates while preparing for action plans and future meetings. Seamlessly approve and distribute comprehensive meeting digests.

To run this app online: [EcoBrand Meeting Minutes Generator Online](https://hero.page/app/ecobrand-meeting-minutes-generator-ai-powered-eco-marketing-meeting-digests/p0CANtljoLAfjvstpUNj)

[![Run EcoBrand Meeting Minutes Generator Online](/assets/run.svg)](https://hero.page/app/ecobrand-meeting-minutes-generator-ai-powered-eco-marketing-meeting-digests/p0CANtljoLAfjvstpUNj)

To learn more about AI Apps for Brand Manager use-cases in the Eco-friendly & Sustainable Product Marketing industry, read [How to Amplify Your Eco-friendly Brand Strategy with AI](https://hero.page/blog/ai/eco-friendly-and-sustainable-product-marketing/how-to-amplify-your-eco-friendly-brand-strategy-with-ai/170848)

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
npx hero run ./ecobrand_meeting_minutes_generator.heroml
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
hero run ./ecobrand_meeting_minutes_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ecobrand_meeting_minutes_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ecobrand_meeting_minutes_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ecobrand_meeting_minutes_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

