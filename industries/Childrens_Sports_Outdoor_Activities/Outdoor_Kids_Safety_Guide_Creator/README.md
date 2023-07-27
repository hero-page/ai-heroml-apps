# Outdoor Kids Safety Guide Creator

Outdoor Kids Safety Guide Creator is an app for creating personalized child outdoor safety guides. Offering AI-powered capabilities, it generates detailed, top-quality safety content specifically for outdoor educators working in children's sports and outdoor activities. It aids in identifying typical hazards, risks, prevention and emergency response techniques in an outdoor setting. The content primarily emphasizes child welfare, readiness for unexpected situations, and includes unique scenarios like high-altitude and water-based activities. Tailored with a focus on teaching safety to children, it's a valuable tool for educators.

To run this app online: [Outdoor Kids Safety Guide Creator Online](https://hero.page/app/outdoor-kids-safety-guide-creator-customized-child-outdoor-safety-guide/aRMKhK3mErk2YzaRFtNq)

[![Run Outdoor Kids Safety Guide Creator Online](/assets/run.svg)](https://hero.page/app/outdoor-kids-safety-guide-creator-customized-child-outdoor-safety-guide/aRMKhK3mErk2YzaRFtNq)

To learn more about AI Apps for Outdoor Educator use-cases in the Children's Sports & Outdoor Activities industry, read [How to Level Up Outdoor Education with AI for Activity Planning, Safety, and Trips](https://hero.page/blog/ai/children's-sports-and-outdoor-activities/how-to-level-up-outdoor-education-with-ai-for-activity-planning-safety-and-trips/170787)

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
npx hero run ./outdoor_kids_safety_guide_creator.heroml
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
hero run ./outdoor_kids_safety_guide_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./outdoor_kids_safety_guide_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./outdoor_kids_safety_guide_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./outdoor_kids_safety_guide_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

