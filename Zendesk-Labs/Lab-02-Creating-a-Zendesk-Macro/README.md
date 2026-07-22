# 🎫 Lab 02 – Creating a Zendesk Macro

## Objective

Learn how to create a reusable Zendesk macro to automate responses to common customer inquiries. This lab demonstrates how macros improve efficiency, maintain consistency across support interactions, and personalize responses using dynamic placeholders.

---

## Skills Practiced

- Zendesk Macros
- Workflow Automation
- Dynamic Placeholders
- IT Service Management (ITSM)
- Customer Communication
- Help Desk Best Practices

---

## Tools Used

- Zendesk Support
- Zendesk Admin Center
- Macros

---

# Lab Walkthrough

## Step 1 – Navigate to the Macros Page

Logged into Zendesk and navigated to the **Admin Center**. From the sidebar, selected **Workspaces** and then **Macros** to access the macro management page.

### Screenshot

*(Insert screenshot of navigating to the Macros page.)*

**Caption**

<sub><em>Navigated to the Zendesk Admin Center and accessed the Macros section to begin creating a reusable support response.</em></sub>

---

## Step 2 – Create a New Macro

Selected **Create Macro** and entered the macro name:

```text
Support: Software Update Steps
```

A descriptive name was chosen to make the macro easy to identify and reuse when responding to software update requests.

### Screenshot

*(Insert screenshot showing the new macro and its title.)*

**Caption**

<sub><em>Created a new macro and assigned a descriptive name to clearly identify its intended support function.</em></sub>

---

## Step 3 – Configure the Macro Response

Entered the response that will automatically populate when the macro is applied to a support ticket.

The response included Zendesk dynamic placeholders to personalize each reply.

```text
Hi {{ticket.requester.first_name}},

Thank you for reaching out! To update your software, please follow these steps:

1. Open the application and go to Settings.
2. Click on Check for Updates.
3. Follow the on-screen prompts to install the latest version.

Let us know if you run into any issues!

Best regards,

{{current_user.first_name}}
```

The placeholders automatically insert:

- The customer's first name
- The responding support agent's first name

This allows the same macro to be reused while still creating a personalized customer experience.

### Screenshot

*(Insert screenshot showing the completed macro response.)*

**Caption**

<sub><em>Configured the macro using dynamic placeholders to automatically personalize responses while maintaining consistent support instructions.</em></sub>

---

## Step 4 – Save the Macro

Reviewed the completed macro for accuracy before saving it. Once saved, the macro became available for future support tickets and could be applied with a single click.

### Screenshot

*(Insert screenshot showing the completed macro after saving.)*

**Caption**

<sub><em>Saved the completed macro, making it available for future customer support requests and improving response efficiency.</em></sub>

---

## What I Learned

Creating Zendesk macros allows support teams to standardize responses for frequently asked questions while reducing repetitive work. By incorporating dynamic placeholders, a single macro can automatically personalize each response using information from the support ticket. This improves response consistency, increases efficiency, and helps deliver a professional customer support experience.

---

## Skills Learned

- Creating reusable Zendesk macros
- Configuring automated support responses
- Using dynamic placeholders for personalization
- Standardizing customer communication
- Improving support workflow efficiency
- Applying automation to common help desk tasks
