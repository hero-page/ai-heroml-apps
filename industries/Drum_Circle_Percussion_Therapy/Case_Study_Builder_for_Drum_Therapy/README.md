# Case Study Builder for Drum Therapy

Immerse yourself in the niche field of Drum Circle & Percussion Therapy with the Case Study Builder for Drum Therapy app. Tailor prompts to your specific needs, allowing the powerful AI to generate custom, in-depth fictional case studies. Review clients' background details, explore therapeutic methods, learn about different percussion instruments used, and witness the impact of therapy on their issues. Develop understanding of a Drum Circle Facilitator's role and outcomes of therapy sessions. Benefit from insights gleaned from anonymized case studies, potentially valuable for future therapy applications.

To run this app online: [Case Study Builder for Drum Therapy Online](https://hero.page/app/case-study-builder-for-drum-therapy-customized-drum-therapy-case-studies/sDMSHniqJEfFgv3ePzLA)

[![Run Case Study Builder for Drum Therapy Online](/assets/run.svg)](https://hero.page/app/case-study-builder-for-drum-therapy-customized-drum-therapy-case-studies/sDMSHniqJEfFgv3ePzLA)

To learn more about AI Apps for Drum Circle Facilitator use-cases in the Drum Circle & Percussion Therapy industry, read [How to Streamline Drum Therapy with AI Tools](https://hero.page/blog/ai/drum-circle-and-percussion-therapy/how-to-streamline-drum-therapy-with-ai-tools/170841)

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
npx hero run ./case_study_builder_for_drum_therapy.heroml
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
hero run ./case_study_builder_for_drum_therapy.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./case_study_builder_for_drum_therapy.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./case_study_builder_for_drum_therapy.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./case_study_builder_for_drum_therapy.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

