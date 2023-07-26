# Numerology Year Forecast Generator

Numerology Year Forecast Generator is an AI-driven mobile app that enables users to generate customized and insightful numerology forecasts. These forecasts are based on a user's birth date and the current year, calculating their Personal Year Number. App users will receive thorough predictions divided into specific life areas like career, relationships, personal growth, and health, offering advice on potential challenges and how to maximise uplifting energies. The forecast is complemented by the inclusion of key numerology elements such as Angel Numbers and Life Path Numbers for an extensive understanding.

To run this app online: [Numerology Year Forecast Generator Online](https://hero.page/app/numerology-year-forecast-generator-ai-powered-personal-numerology-forecasts/KS92sZ1Lvp2k1vb3PQvS)

To learn more about AI Apps for Numerologist use-cases in the Astrology & Numerology industry, read [How to Generate Comprehensive Numerology Reports with AI Apps](https://hero.page/blog/ai/astrology-and-numerology/how-to-generate-comprehensive-numerology-reports-with-ai-apps/170740)

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
npx hero run ./numerology_year_forecast_generator.heroml
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
hero run ./numerology_year_forecast_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./numerology_year_forecast_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./numerology_year_forecast_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./numerology_year_forecast_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Numerology Year Forecast Generator
```
Write a "Personal Year Forecast" for the "Astrology & Numerology" industry, specifically for a "Numerologist". 

First, we'll start with an introduction that explains what a "Personal Year Forecast" is. It should explain how it provides insights into the year ahead regarding areas like personal, professional, and spiritual growth. 

Here's some more context about the Personal Year Forecast:
Introduction: {{introduction}}
Birth Date: {{birth_date}}
Universal Year Number: {{Universal_Year_Number}}
Personal Year Overview: {{Personal_Year_Overview}}
Career Forecast: {{Career_Forecast}}
Relationships Forecast: {{Relationships_Forecast}}
Personal Growth Forecast: {{Personal_Growth_Forecast}}
Health Forecast: {{Health_Forecast}}
Life Advice: {{life_advice}}
Summary: {{summary}}

->>>>

For the "Personal Year Forecast", we have constructed the following introduction:

Introduction:
{{step_1}}

Now, let's explain how to calculate the Personal Year Number using the user's birth date. The user's birth date (day and month) plus the Universal Year number (current year reduced to a single digit) equals their Personal Year Number.

->>>>

For the "Personal Year Forecast", we have defined the method to calculate the Personal Year Number:

Introduction:
{{step_1}}

Method to Calculate Personal Year Number:
{{step_2}}

Our next task is to provide an overview of what that Personal Year in numerology represents generally, from an overall perspective.

->>>>

For the "Personal Year Forecast", we have constructed an overview:

Introduction:
{{step_1}}

Method to Calculate Personal Year Number:
{{step_2}}

Personal Year Overview:
{{step_3}}

Now, let's section the forecast into areas like career, relationships, personal growth, and health. For each of these sections, we need to provide detailed predictions relevant to their Personal Year Number.

->>>>

In our "Personal Year Forecast", we have detailed predictions for each specific domain:

Personal Year Overview:
{{step_3}}

Career Forecast:
{{step_4a}}

Relationships Forecast:
{{step_4b}}

Personal Growth Forecast:
{{step_4c}}

Health Forecast:
{{step_4d}}

Next, we have to offer guidance on how the reader can navigate potential challenges and how best to utilize the positive energy in their Personal Year. This should provide practical life advice based on their Personal Year Number.

->>>>

In our "Personal Year Forecast", we have provided life advice based on the Personal Year Number:

Career Forecast:
{{step_4a}}

Relationships Forecast:
{{step_4b}}

Personal Growth Forecast:
{{step_4c}}

Health Forecast:
{{step_4d}}

Life Advice:
{{step_5}}

For the conclusion, let's summarize the forecast, reminding them of their Personal Year Number and its key themes, and encouraging them to use this forecast as a tool for personal development.


```

