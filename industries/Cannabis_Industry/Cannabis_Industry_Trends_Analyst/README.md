# Cannabis Industry Trends Analyst

Get exclusive insights into the cannabis industry with the Cannabis Industry Trends Analyst app! Uncover latest market dynamics with AI-generated, customized trend reports. Define variables for detailed analysis like driving factors, competitive landscape, regulatory impact, growth opportunities, industry challenges, and future forecasts-specific to cannabis industry. Ideal for consultants seeking comprehensive, high-quality cannabis industry data.

To run this app online: [Cannabis Industry Trends Analyst Online](https://hero.page/app/cannabis-industry-trends-analyst-cannabis-market-insight-generation/wPA19Ry3SBIrzhZjRjRC)

[![Run Cannabis Industry Trends Analyst Online](/assets/run.svg)](https://hero.page/app/cannabis-industry-trends-analyst-cannabis-market-insight-generation/wPA19Ry3SBIrzhZjRjRC)

To learn more about AI Apps for Industry Consultant use-cases in the Cannabis Industry industry, read [How to Exploit AI for In-depth Cannabis Market Analysis](https://hero.page/blog/ai/cannabis-industry/how-to-exploit-ai-for-in-depth-cannabis-market-analysis/170771)

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
npx hero run ./cannabis_industry_trends_analyst.heroml
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
hero run ./cannabis_industry_trends_analyst.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./cannabis_industry_trends_analyst.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./cannabis_industry_trends_analyst.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./cannabis_industry_trends_analyst.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Cannabis Industry Trends Analyst
```
Your task is to write an "Industry Trends Report" for the "Cannabis Industry" industry, specifically for an "Industry Consultant". Let's start by generating an executive summary that succinctly explains the overall trends in the cannabis industry: {{overall_trends}}.

Here's some more context about the Industry Trends Report:
Overall Trends: {{overall_trends}}
Key Market Drivers: {{key_market_drivers}}
Competitive Landscape: {{competitive_landscape}}
Regulatory Changes: {{regulatory_changes}}
Industry Segments Growth Opportunities: {{industry_segments_growth_opportunities}}
Industry Challenges: {{industry_challenges}}
Future Trajectories: {{future_trajectories}}
Dynamic Variable: {{dynamic_variable}}

->>>>

We have an executive summary that explains the current trends:

Executive Summary:
{{step_1}}

Next, let's write a detailed introduction that provides a brief history and present state of the cannabis industry.

->>>>

By now we have an executive summary and a detailed introduction:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Let's proceed to the first section of the report. In this section, identify and discuss key market-drivers in the cannabis industry: {{key_market_drivers}}.

->>>>

After explaining the history and present state of the cannabis industry, we now have a section on key market-drivers:

Introduction:
{{step_2}}

Key Market-Drivers:
{{step_3}}

For the second section, let's analyze the competitive landscape in the cannabis industry: {{competitive_landscape}}.

->>>>

With a section on key market-drivers, we now have an analysis of the competitive landscape:

Key Market-Drivers:
{{step_3}}

Competitive Landscape:
{{step_4}}

In the third section of the report, let's highlight significant regulatory changes and their potential impacts on the cannabis industry: {{regulatory_changes}}.

->>>>

While continuing with the trends report, after analyzing the competitive landscape, discuss the regulatory changes:

Competitive Landscape:
{{step_4}}

Regulatory Changes:
{{step_5}}

The fourth section should explore growth opportunities specific to different industry segments: {{industry_segments_growth_opportunities}}.

->>>>

Having detailed the regulatory changes, we now have an exploration of the growth opportunities:

Regulatory Changes:
{{step_5}}

Growth Opportunities:
{{step_6}}

Now, let's discuss the key challenges facing the cannabis industry: {{industry_challenges}}.

->>>>

After exploring growth opportunities, let's delve into the key challenges of the cannabis industry:

Growth Opportunities:
{{step_6}}

Industry Challenges:
{{step_7}}

In the conclusion, let's summarize the major takeaways and present future trajectories for the cannabis industry based on the trends outlined in the report: {{future_trajectories}}.


```

