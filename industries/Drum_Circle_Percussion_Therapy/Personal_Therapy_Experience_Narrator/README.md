# Personal Therapy Experience Narrator

Experience a unique journey into the world of drum therapy with the Personal Therapy Experience Narrator. Your individual experiences are transformed into an engaging narrative by our advanced AI. This app allows you to customize your prompts, capturing the vivid ambiance of your session, the drums used, and community interactions. It goes beyond just sharing facts, as it recollects your personal emotions and therapeutic benefits from your session. The narrative concludes with a summary of your journey, offering potential recommendations. Thus, providing a wholesome, immersive experience in Drum Circle & Percussion Therapy.

To run this app online: [Personal Therapy Experience Narrator Online](https://hero.page/app/personal-therapy-experience-narrator-customized-drum-therapy-narratives/kW2WWaYnW1ufiRatoI9h)

[![Run Personal Therapy Experience Narrator Online](/assets/run.svg)](https://hero.page/app/personal-therapy-experience-narrator-customized-drum-therapy-narratives/kW2WWaYnW1ufiRatoI9h)

To learn more about AI Apps for Wellness Blogger use-cases in the Drum Circle & Percussion Therapy industry, read [How to Enhance Drum Circle Therapy Blogging with AI Tools](https://hero.page/blog/ai/drum-circle-and-percussion-therapy/how-to-enhance-drum-circle-therapy-blogging-with-ai-tools/170842)

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
npx hero run ./personal_therapy_experience_narrator.heroml
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
hero run ./personal_therapy_experience_narrator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./personal_therapy_experience_narrator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./personal_therapy_experience_narrator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./personal_therapy_experience_narrator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```
