# Personalized Birth Chart Analysis AI

Unveil your cosmos influenced persona with our AI-Powered Personalized Birth Chart Analysis app. Personalize prompts with birth details for a custom-made astrological profile–detailing Sun, Moon and Rising signs. The AI analyses the celestial placements and their interconnections, alongside unique chart features and the North and South Nodes. Uncover a comprehensive, intricate analysis imparting profound insight into the core character, emotions, life path, challenges and hidden triumphs. A detailed, all-encompassing astrological journey awaits.

To run this app online: [Personalized Birth Chart Analysis AI Online](https://hero.page/app/personalized-birth-chart-analysis-ai-ai-powered-custom-astrology-profile/oiYYaXyKUN6r3ZFeyAOE)

[![Run Personalized Birth Chart Analysis AI Online](/assets/run.svg)](https://hero.page/app/personalized-birth-chart-analysis-ai-ai-powered-custom-astrology-profile/oiYYaXyKUN6r3ZFeyAOE)

To learn more about AI Apps for Astrologer use-cases in the Astrology & Numerology industry, read [How to Elevate Horoscope Creation with AI Astrology Apps](https://hero.page/blog/ai/astrology-and-numerology/how-to-elevate-horoscope-creation-with-ai-astrology-apps/170739)

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
npx hero run ./personalized_birth_chart_analysis_ai.heroml
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
hero run ./personalized_birth_chart_analysis_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./personalized_birth_chart_analysis_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./personalized_birth_chart_analysis_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./personalized_birth_chart_analysis_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Personalized Birth Chart Analysis AI
```
Your task is to write a "Birth Chart Analysis" for the "Astrology & Numerology" industry, specifically for an "Astrologer". Let's start by drafting an introductory paragraph explaining the individual's {{birth_date}} and {{birth_time}}, and the significance of these factors in a birth chart analysis.

Here's some more context about the Birth Chart Analysis:
Birth Date: {{birth_date}}
Birth Time: {{birth_time}}
Individual Name: {{individual_name}}
Birth Place: {{birth_place}}

->>>>

We begin the "Birth Chart Analysis" with an introduction:

Introduction:
{{step_1}}

Next, let's describe the Sun sign – the Zodiac sign that the Sun was traveling through at the exact {{birth_time}} and {{birth_date}}. Explain what the Sun sign implies about {{individual_name}}'s core self, basic personality, and ego.

->>>>

In the "Birth Chart Analysis", we have an introduction and a description of Sun sign:

Introduction:
{{step_1}}

Sun Sign Description:
{{step_2}}

Now, analyze {{individual_name}}'s Moon sign - the Zodiac sign where the Moon was stationed at the time of birth. Interpret how this reveals the individual's emotional and inner world.

->>>>

In our "Birth Chart Analysis", we have a description of the Sun sign and a detailed analysis of the Moon sign:

Sun Sign Description:
{{step_2}}

Moon Sign Analysis:
{{step_3}}

Next, discuss the Ascendant (or Rising sign), which represents the sign that was coming up on the Eastern horizon at the {{birth_time}} in the {{birth_place}}. This section should delve into how {{individual_name}} presents himself or herself to the external world.

->>>>

For the "Birth Chart Analysis", we have analyzed Moon sign and explained the Ascendant:

Moon Sign Analysis:
{{step_3}}

Ascendant Explanation:
{{step_4}}

Now, it's time to do a detailed rundown of every planet (Mercury, Venus, Mars, Jupiter, Saturn, Uranus, Neptune, and Pluto) and their respective house positions at the {{birth_time}} and {{birth_date}}. Explain how these affect various aspects of {{individual_name}}'s life including communication style, love tendencies, drive, luck, discipline, rebellion, dreams, power, etc.

->>>>

In our "Birth Chart Analysis", we have explained the Ascendant and given a detailed analysis of each planet and its house position:

Ascendant Explanation:
{{step_4}}

Planets and House Positions Analysis:
{{step_5}}

Analyze the Angular relationships (or ‘aspects’) between the planets at the time of birth. Discuss whether any patterns ('Yods', 'T-Squares' etc.) are formed, and what they signify for {{individual_name}}.

->>>>

In our "Birth Chart Analysis", we have analyzed each planet and its house position and the Angular relationships between the planets:

Planets and House Positions Analysis:
{{step_5}}

Angular Relationships Analysis:
{{step_6}}

Next, explain the North Node and South Node, which are the points where the moon's orbit crosses the ecliptic at the {{birth_date}} and {{birth_time}}, and provide insights into the life path that {{individual_name}} is meant to take and their past lives respectively.

->>>>

In our "Birth Chart Analysis", we have analyzed Angular relationships between the planets and provided an explanation of the North Node and South Node:

Angular Relationships Analysis:
{{step_6}}

North Node and South Node Explanation:
{{step_7}}

If the birth chart showcases any unique features (like stelliums, grand trines, etc), discuss their implications on the individual's life.


```

