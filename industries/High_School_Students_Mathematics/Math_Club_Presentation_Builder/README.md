# Math Club Presentation Builder

Math Club Presentation Builder is an AI-powered tool designed to produce bespoke math presentations for high school clubs. Users can define variables in prompts, allowing the app to generate content that's both engaging and educational. Showcasing specific math topics, the app makes relevant real-world applications and includes Math Competition problems, spurring interactive problem-solving. Main points are summarized, followed by a Q&A section to encourage dialogue. For further exploration, the app provides additional resources. Its unique attribute is its tailored approach to delivering math presentations that are both instructional and engaging.

To run this app online: [Math Club Presentation Builder Online](https://hero.page/app/math-club-presentation-builder-interactive-math-presentation-generator/PYvXDzRs4yJiHYE6Ja39)

[![Run Math Club Presentation Builder Online](/assets/run.svg)](https://hero.page/app/math-club-presentation-builder-interactive-math-presentation-generator/PYvXDzRs4yJiHYE6Ja39)

To learn more about AI Apps for Math Club Member use-cases in the High School Students - Mathematics industry, read [How to Excel in Math Competitions with AI-Powered Apps](https://hero.page/blog/ai/high-school-students-mathematics/how-to-excel-in-math-competitions-with-ai-powered-apps/170960)

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
npx hero run ./math_club_presentation_builder.heroml
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
hero run ./math_club_presentation_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./math_club_presentation_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./math_club_presentation_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./math_club_presentation_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

