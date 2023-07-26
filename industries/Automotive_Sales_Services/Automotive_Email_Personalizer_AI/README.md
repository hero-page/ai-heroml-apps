# Automotive Email Personalizer AI

Explore Automotive Email Personalizer AI, an app specialized in creating intimately personalized, informative, & convincing emails aimed at automotive sales & services clientele. Emphasize on personal connection, coupled with insightful & promotional content. Craft bespoke emails introducing personalized greetings, company info, automotive services, industry insights & more. This AI-driven app enhances customer engagement while promoting services in a professional and comprehensive manner.

To run this app online: [Automotive Email Personalizer AI Online](https://hero.page/app/automotive-email-personalizer-ai-personalized-auto-service-connect/OFrIca8tQOQrn5kJPyEf)

To learn more about AI Apps for Automotive Technician use-cases in the Automotive Sales & Services industry, read [How to Enhance Auto Repair Estimates, Service Reports and Client Emails with AI](https://hero.page/blog/ai/automotive-sales-and-services/how-to-enhance-auto-repair-estimates-service-reports-and-client-emails-with-ai/170749)

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
npx hero run ./automotive_email_personalizer_ai.heroml
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
hero run ./automotive_email_personalizer_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./automotive_email_personalizer_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./automotive_email_personalizer_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./automotive_email_personalizer_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Automotive Email Personalizer AI
```
Your task is to write a "Customer Email" for the "Automotive Sales & Services" industry, specifically for an "Automotive Technician". 

Let's start with composing a greeting that addresses the customer directly: "Dear {{customer_name}}".

Here's some more context about the Customer Email:
Customer Name: {{customer_name}}
Technician Name: {{technician_name}}
Company Name: {{company_name}}
Vehicle Types: {{vehicle_types}}
Vehicle Type: {{vehicle_type}}

->>>>

We're starting the Customer Email:

Greetings:
{{step_1}}

Now, initiate the conversation by expressing gratitude and extending appreciation for considering your automotive services: "We appreciate your interest in our services...".

->>>>

So far we have the greeting and the conversation initiation:

Greetings:
{{step_1}}

Initiating Conversation:
{{step_2}}

Next, provide a brief introduction about yourself, the company, and the unique automotive services you offer: "I am {{technician_name}}, a certified automotive technician at {{company_name}}...".

->>>>

Currently, our customer email has the greeting, initiation, and a brief introduction:

Greetings:
{{step_1}}

Initiating Conversation:
{{step_2}}

Introduction:
{{step_3}}

Let's clearly describe how your services could meet the customer's needs. This should include the type of vehicles you service, special expertise, quality guarantees, and promotions: "At {{company_name}}, we service {{vehicle_types}}...".

->>>>

In our Customer Email, we now have a description of services added after the introduction:

Introduction:
{{step_3}}

Service Description:
{{step_4}}

Next, incorporate industry-specific elements by discussing any upcoming advancements, challenges, or trends in the automotive industry which could impact their vehicle's performance or maintenance requirements: "There have been significant advancements in automotive technology...".

->>>>

Our email now also contains information about industry-specific elements:

Service Description:
{{step_4}}

Industry-Specific Information:
{{step_5}}

Let's encourage the customer to book an appointment or service. Be specific about the process like online scheduling or calling the service center: "To schedule an appointment...".

->>>>

Now, our email contains the next step for the customer:

Industry-Specific Information:
{{step_5}}

Appointment Invitation:
{{step_6}}

To end, reassure the customer of excellent service and look forward to their response: "We look forward to servicing your {{vehicle_type}}...". Also, provide an opportunity for the customer to ask any questions they may have: "Feel free to ask any queries...".

->>>>

The email now concludes with a reassurance of service:

Appointment Invitation:
{{step_6}}

Service Reassurance:
{{step_7}}

Finally, close the email with professional ending salutations, your full name, position, and contact details: "Best Regards, {{technician_name}}".


```

