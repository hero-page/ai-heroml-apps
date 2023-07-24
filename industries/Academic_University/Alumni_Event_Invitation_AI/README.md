# Alumni Event Invitation AI

Alumni Event Invitation AI is a revolutionary app that leverages AI technology to create highly customized event invitations, specifically tailored for Alumni Relations Officers in the Academic & University realm. Users can specify essential variables in prompts such as date, time, and venue. More than listing basic event details, the app crafts details about the event's purpose and relation to alumni, introduces keyguest speakers, highlights attractions, outlines benefits for alumni attendees, and explains RSVP details, including pre-registration requirements or costs. The tailored content amplifies the invitation's relevance and effectiveness, stepping beyond generic invitations.

To run this app online: [Alumni Event Invitation AI Online](https://hero.page/app/alumni-event-invitation-ai-ai-powered-personalized-alumni-invitations/DXl9DpMVO5QHyDKem2WB)

To learn more about AI Apps for Alumni Relations Officer use-cases in the Academic & University industry, read [How to Elevate Alumni Outreach with AI-powered Newsletter, Fundraising and Event Invites](https://hero.page/blog/academic-and-university/alumni-relations-officer/how-to-elevate-alumni-outreach-with-ai-powered-newsletter-fundraising-and-event-invites/170710)

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
npx hero run ./alumni_event_invitation_ai.heroml
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
hero run ./alumni_event_invitation_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./alumni_event_invitation_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./alumni_event_invitation_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./alumni_event_invitation_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Alumni Event Invitation AI
```
Your task is to write a "Event Invitation" for the "Academic & University" industry, specifically for an "Alumni Relations Officer". 
Let's begin by writing a warm introductory statement which highlights the purpose of the event and its relevance to the alumni: {{event_purpose}}. 

Here's some more context about the Event Invitation:
Event Purpose: {{event_purpose}}
Event Details: {{event_details}}
Event Highlights: {{event_highlights}}
Guest Speakers: {{guest_speakers}}
Alumni Benefits: {{alumni_benefits}}
RSVP Information: {{RSVP_information}}

->>>>

We have started our invitation with an engaging introduction:

Introduction:
{{step_1}}

Next, write a detailed section describing the event. Include key information such as the event's date, time, and venue: {{event_details}}.

->>>>

Our invitation now has an engaging introduction and a comprehensive description of the event details:

Introduction:
{{step_1}}

Event Details:
{{step_2}}

Let's move on to creating a section covering the main highlights of the event and giving attendees an idea of what they can expect: {{event_highlights}}.

->>>>

We have an introduction, event details, and highlights for our invitation:

Introduction:
{{step_1}}

Event Details:
{{step_2}}

Event Highlights:
{{step_3}}

Next, mention the names and any notable achievements of the key speakers or guests who will be attending: {{guest_speakers}}.

->>>>

At this point, we have an introduction, event details, highlights, and guest speaker information for our invitation:

Introduction:
{{step_1}}

Event Details:
{{step_2}}

Event Highlights:
{{step_3}}

Guest Speakers:
{{step_4}}

Let's build a section urging alumni to attend, explaining why their presence is valuable and what attending might mean for them: {{alumni_benefits}}.

->>>>

So far, our invitation includes an introduction, event details, highlights, guest speaker information and a section encouraging alumni attendance:

Introduction:
{{step_1}}

Event Details:
{{step_2}}

Event Highlights:
{{step_3}}

Guest Speakers:
{{step_4}}

Appeal to Alumni:
{{step_5}}

To finalize the invitation, provide an RSVP conclusion with details on responding, any prerequisites for attendance like pre-registration or fees: {{RSVP_information}}.


```

