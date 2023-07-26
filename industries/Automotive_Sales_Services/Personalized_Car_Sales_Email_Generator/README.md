# Personalized Car Sales Email Generator

Experience seamless car salesmanship with the Personalized Car Sales Email Generator, an AI-powered tool that crafts high-quality, customized emails. As a user, specify variables in prompts to align with your prospective buyer's needs. The app will generate a compelling email complete with an attention-grabbing subject line, a detailed car description, enticing value proposition, an attractive pricing or financing offer and a befitting call-to-action. It's signature feature - a professional, personalized email that aligns with industry terms and is authentic and human-like, whilst maintaining transparency throughout.

To run this app online: [Personalized Car Sales Email Generator Online](https://hero.page/app/personalized-car-sales-email-generator-ai-powered-personalized-car-sales-emails/7AUABgXNkAwsyJnbb6DO)

To learn more about AI Apps for Car Salesperson use-cases in the Automotive Sales & Services industry, read [How to Enhance Car Sales with AI-Driven Descriptions, Emails, and Summaries](https://hero.page/blog/ai/automotive-sales-and-services/how-to-enhance-car-sales-with-ai-driven-descriptions-emails-and-summaries/170748)

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
npx hero run ./personalized_car_sales_email_generator.heroml
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
hero run ./personalized_car_sales_email_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./personalized_car_sales_email_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./personalized_car_sales_email_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./personalized_car_sales_email_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Personalized Car Sales Email Generator
```
Your task is to write a "Sales Email" for the "Automotive Sales & Services" industry, specifically for a "Car Salesperson".

Let's start with Step 1: Initiate the Email

We need to begin the sales email with a short, compelling subject line to encourage readers to open the email and discover more. 

Here's some more context about the Sales Email:
Subject Line: {{subject_line}}
Recipient Name: {{recipient_name}}
Car Details: {{car_details}}
Value Proposition: {{value_proposition}}
Offer Details: {{offer_details}}
Call To Action: {{call_to_action}}
Signature: {{signature}}

->>>>

For our "Sales email" we have a compelling subject line:

Subject line:
{{step_1}}

For Step 2: Introduction

We should open the body of the email with a warm greeting and an introduction, briefly explaining the purpose of the email. Within the introduction, address the recipient by their name.

->>>>

For our "Sales Email", we have a compelling subject line and introduction:

Subject line:
{{step_1}}

Introduction:
{{step_2}}

Moving to Step 3: Detailing the Product or Offer 

We need to get into specifics about the vehicle in question: model, year, features, and condition. Emphasize any unique selling points of the car that might attract the buyer.

->>>>

For our "Sales Email", we have a compelling subject line, an introduction and detailed product specification:

Subject line:
{{step_1}}

Introduction:
{{step_2}}

Car Details:
{{step_3}}

Now to Step 4: Demonstrate Value

We express why this specific vehicle suits the recipient's needs by alluding to their previously expressed preferences or requirements. Consider fuel efficiency, safety features or any other aspect of importance to the prospective buyer.

->>>>

For our "Sales Email", we have a compelling subject line, an introduction, product specification, and demonstrated value:

Subject line:
{{step_1}}

Introduction:
{{step_2}}

Car Details:
{{step_3}}

Value Proposition:
{{step_4}}

Moving on to Step 5: Sharing the Offer

We inform the prospect about the price or financing offer for the vehicle, include any promotional deals or service packages that come with the purchase. Be careful to remain transparent about all costs.

->>>>

For our "Sales Email", we have a compelling subject line, an introduction, product specification, demonstrated value, and a presented offer:

Subject line:
{{step_1}}

Introduction:
{{step_2}}

Car Details:
{{step_3}}

Value Proposition:
{{step_4}}

Offer Details:
{{step_5}}

Now for Step 6: CTA (Call to Action)

We conclude your sales email with a clear and direct call to action (CTA). This could be inviting the customer to a test drive, a phone call for more details, or a visit to your showroom.

->>>>

For our "Sales Email", we have a compelling subject line, an introduction, product specification, demonstrated value, a presented offer and a call to action:

Subject line:
{{step_1}}

Introduction:
{{step_2}}

Car Details:
{{step_3}}

Value Proposition:
{{step_4}}

Offer Details:
{{step_5}}

Call to Action:
{{step_6}}

Finally, for Step 7: Signature

We have to sign off the email professionally including your full name, position, contact details, and dealership information.


```

