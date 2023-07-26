# Press Release Storyteller AI

Create engaging marketing narratives with Press Release Storyteller AI that uses AI to generate press releases. Users can specify variables in prompts for a customized, high-quality output. The app crafts detailed stories of a company's significant updates, supported by key personnel quotes and statistics, amongst other details. All aimed at capturing media attention. The unique aspect is that it doesn't just report news, but crafts an informative story to stir positive discussions.

To run this app online: [Press Release Storyteller AI Online](https://hero.page/app/press-release-storyteller-ai-ai-powered-marketing-storytelling/sgJSShIi6Dc4iRRnkLO3)

[![Run Press Release Storyteller AI Online](/assets/run.svg)](https://hero.page/app/press-release-storyteller-ai-ai-powered-marketing-storytelling/sgJSShIi6Dc4iRRnkLO3)

To learn more about AI Apps for Marketing Manager use-cases in the Advertising & Marketing industry, read [How to Transform Marketing Strategy with Top AI Workflow Apps](https://hero.page/blog/ai/advertising-and-marketing/how-to-transform-marketing-strategy-with-top-ai-workflow-apps/170718)

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
npx hero run ./press_release_storyteller_ai.heroml
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
hero run ./press_release_storyteller_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./press_release_storyteller_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./press_release_storyteller_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./press_release_storyteller_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Press Release Storyteller AI
```
Your task is to write a "Press Release" for the "Advertising & Marketing" industry, specifically for a "Marketing Manager".

Let's begin with an attention-grabbing headline. The headline should clearly state the main point of the press release: {{headline_point}}. It needs to be catchy enough to grab the attention of journalists, while being informative and providing a snapshot of the news being announced.

Here's some more context about the Press Release:
Headline Point: {{headline_point}}
News Details: {{news_details}}
Company Intro: {{company_intro}}
News Specifics: {{news_specifics}}
Relevant Statistics: {{relevant_statistics}}

->>>>

For our Press Release we have the following headline:

Headline:
{{step_1}}

Next, we need a subheading or lead paragraph that provides more details about the news: {{news_details}}. It should offer necessary context and arouse the reader's curiosity to continue reading.

->>>>

Our Press Release now has a title and lead paragraph:

Headline:
{{step_1}}

Lead Paragraph:
{{step_2}}

Now, let's add a dateline, indicating the location and date of the press release to provide it a time context.

->>>>

Our Press Release so far:

Headline:
{{step_1}}

Lead Paragraph:
{{step_2}}

Dateline:
{{step_3}}

Next, the body of the press release should begin with a brief introduction of the company: {{company_intro}}. This section will provide necessary background information for anyone who is not familiar with your organization.

->>>>

Our updated Press Release is as follows:

Dateline:
{{step_3}}

Company Introduction:
{{step_4}}

Our main task is to detail the specifics of the news we are announcing: {{news_specifics}}. This section should be factual and straightforward. Ensure to use simple language and avoid industry jargon.

->>>>

We now have a detailed part of our Press Release:

Company Introduction:
{{step_4}}

News Details:
{{step_5}}

We need to add a quotation from a high-ranking company official, like the CEO or the Marketing Manager. This quote should provide a human touch, express the company's viewpoint, or elaborate on the significance of the news.

->>>>

We have the following for our Press Release:

News Details:
{{step_5}}

Quotation:
{{step_6}}

Now, any relevant data or statistics related to the news: {{relevant_statistics}} should be included to reinforce the message and add credibility to the press release.

->>>>

Our Press Release now has the following sections:

Quotation:
{{step_6}}

Relevant Statistics:
{{step_7}}

Let's briefly mention company achievements related to the news to exhibit industry standing or significance.

->>>>

The updated state of our Press Release is:

Relevant Statistics:
{{step_7}}

Company Achievements:
{{step_8}}

Now we will add a standard company boilerplate – a brief paragraph about the company, which includes its mission, key offerings, year of establishment, etc. This part is reusable and can be included in all press releases.

->>>>

Our Press Release now includes:

Company Achievements:
{{step_8}}

Company Boilerplate:
{{step_9}}

Finally, provide the contact information of the person whom journalists can reach out to for more information or clarification.


```

