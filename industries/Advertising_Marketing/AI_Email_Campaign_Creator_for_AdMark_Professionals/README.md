# AI Email Campaign Creator for AdMark Professionals

The AI Email Campaign Creator for AdMark Professionals app crafts tailored content for advertising professionals. Users can specify variables to generate compelling subject lines, greetings, insightful main bodies, and action calls. The unique feature targets industry professionals, emphasizing sender's product benefits and relevant industry trends, fostering better audience engagement and resonance.

To run this app online: [AI Email Campaign Creator for AdMark Professionals Online](https://hero.page/app/ai-email-campaign-creator-for-admark-professionals-admark-content-and-insight-generator/sOkBpq0QcjHA2CPDHozp)

[![Run AI Email Campaign Creator for AdMark Professionals Online](/assets/run.svg)](https://hero.page/app/ai-email-campaign-creator-for-admark-professionals-admark-content-and-insight-generator/sOkBpq0QcjHA2CPDHozp)

To learn more about AI Apps for Copywriter use-cases in the Advertising & Marketing industry, read [How to Supercharge Ad Creation, Email Campaigns, and Blog Posts with AI](https://hero.page/blog/ai/advertising-and-marketing/how-to-supercharge-ad-creation-email-campaigns-and-blog-posts-with-ai/170716)

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
npx hero run ./ai_email_campaign_creator_for_admark_professionals.heroml
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
hero run ./ai_email_campaign_creator_for_admark_professionals.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ai_email_campaign_creator_for_admark_professionals.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ai_email_campaign_creator_for_admark_professionals.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ai_email_campaign_creator_for_admark_professionals.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for AI Email Campaign Creator for AdMark Professionals
```
Your task is to write an "Email Campaign" for the "Advertising & Marketing" industry, specifically for a "Copywriter". 

To begin, let's craft a compelling subject line that piques the interest of your target recipients.

Here's some more context about the Email Campaign:
Subject Line: {{subject_line}}
Opening Salutation: {{opening_salutation}}
Email Purpose: {{email_purpose}}
Main Content: {{main_content}}
Value Proposition: {{value_proposition}}
Call To Action: {{call_to_action}}
Closing Statement: {{closing_statement}}

->>>>

We have a compelling subject line for our email campaign:

Subject Line:
{{step_1}}

Next, construct the opening of your email with a personalized salutation and a warm introduction that establishes a rapport with the recipient and sets the tone for the email.

->>>>

The subject line and the opening for our email is ready:

Subject Line:
{{step_1}}

Opening Salutation:
{{step_2}}

Next, state the purpose of the email and briefly outline what will be discussed in the upcoming sections.

->>>>

We have created our email's subject, opening, and purpose:

Subject Line:
{{step_1}}

Opening Salutation:
{{step_2}}

Email Purpose:
{{step_3}}

Now, carry on with the main body of your content. This part of the email should be informative, disseminating useful insights or knowledge pertinent to the industry.

->>>>

Our email so far has a subject line, opening, purpose and now, the main body:

Subject Line:
{{step_1}}

Opening Salutation:
{{step_2}}

Email Purpose:
{{step_3}}

Main Content:
{{step_4}}

Carry on to showcase specific benefits or value propositions that differentiate your service or product, and pinpoint any industry-specific trends or challenges.

->>>>

On our email now, we have a detailed introduction, main body, and we highlighted the benefits or value propositions:

Introduction and Email Purpose:
{{step_3}}

Main Content:
{{step_4}}

Value Proposition:
{{step_5}}

Let's proceed to the call to action (CTA). This may involve asking the recipient to reply to your email, visit your website, download a resource, or maybe sign up for a demo or a consultation.

->>>>

Currently, we have the main content along with the value proposition and a call to action:

Main Content:
{{step_4}}

Value Proposition:
{{step_5}}

Call to Action:
{{step_6}}

To wrap things up, create a polite sign-off, a reminder of the CTA, and your contact details - making it easy for the recipient to get in touch if they wish.


```

