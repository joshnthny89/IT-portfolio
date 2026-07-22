# 🎫 Lab 02 – Creating a Zendesk Macro

## Objective

Learn how to create a reusable Zendesk macro that provides consistent, professional responses to common customer inquiries while utilizing dynamic placeholders to personalize each response.

---

## Skills Practiced

- Zendesk Macros
- Workflow Automation
- Dynamic Placeholders
- Help Desk Best Practices
- Customer Communication

---

## Tools Used

- Zendesk Support
- Zendesk Macros

---

# Lab Walkthrough

## Step 1 – Navigate to the Macro Administration Page

Opened the Zendesk Admin Center and navigated to the Macros section.

### Screenshot

*(Insert screenshot.)*

**Caption**

<sub><em>Navigated to the Zendesk Macros section to create a reusable support response.</em></sub>

---

## Step 2 – Create a New Macro

Created a new macro named:

```text
Support: Software Update Steps
```

### Screenshot

*(Insert screenshot.)*

**Caption**

<sub><em>Created a new Zendesk macro to automate responses for common software update requests.</em></sub>

---

## Step 3 – Configure the Macro

Added the response text including dynamic placeholders.

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

### Screenshot

*(Insert screenshot.)*

**Caption**

<sub><em>Configured the macro using Zendesk placeholders to automatically personalize each response.</em></sub>

---

## Step 4 – Save the Macro

Saved the completed macro for future use.

### Screenshot

*(Insert screenshot.)*

**Caption**

<sub><em>Saved the completed macro, making it available for future support tickets.</em></sub>

---

## What I Learned

Creating macros allows support teams to automate repetitive responses while maintaining consistency, reducing response times, and improving the overall customer experience through dynamic personalization.
