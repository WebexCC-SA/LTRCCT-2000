#icon: material/folder-open-outline
icon: material/medal
---
## Feature Description

The Webex Contact Center Wrap-up Summary AI feature is part of the AI Assistant capabilities designed to enhance agent productivity and customer experience. This feature automatically generates the conversations summaries based on the interactions between the agent and the customer during a contact center session. It helps agents by summarizing the conversation and recommending next actions, reducing manual effort and improving accuracy in post-call documentation. 

Benefits:

**Reduced agent workload**: By automatically generating wrap-up codes and summarizing conversations, agents spend less time on manual documentation.<br/>
**Improved accuracy**: The AI-generated summaries and codes help ensure consistent and precise post-call records.<br/>
**Enhanced customer satisfaction**: Thorough and accurate wrap-up improves follow-up actions and overall customer experience.<br/>
**Increased agent efficiency**: Integration with other AI capabilities like virtual agent summaries and suggested responses helps agents work more effectively.<br/>
**Recommended next actions**: The feature suggests follow-up steps, guiding agents on what to do after the interaction.<br/>


## Mission Details

Your mission is to:

1. Enable Wrap-up Summary feature
2. Test Wrap-up Summary feature


## Build

### Task 1 <span style="color: red;">[READ ONLY]</span>. Order Provisioning & Control Hub Settings

1. You should purchase the new AI Assistant SKU **A-FLEX-AI-ASST** from CCW.

2. Currently, Wrap-up Summary is not even in early access, so you will not be able to see its enablement in the Control Hub. However, once the feature is in General Access, you will see the toggle under the General Summaries section.
   ![Profiles](../graphics/Lab1_AI_Agent/3.45.png)

3. The Agent needs to logged in to the Team that is configured with Desktop Layout that has Agent Assistance features configured. Default desktop layout already incude the AI Agent Assistance widget.
    <br/>Agents Team:
   ![Profiles](../graphics/Lab1_AI_Agent/3.41.png)    
    <br/>Desktop Layout:
   ![Profiles](../graphics/Lab1_AI_Agent/3.43.png) 


### Task 2. Test Wrap-up Summary feature.

1. This feature is currently is only available in alpha desktop version. Open up new window in your browser and enter the the URL: ***<copy>https://alpha-desktop.wxcc-us1.cisco.com</copy>***.
   ![Profiles](../graphics/Lab1_AI_Agent/3.46.gif)

2. Make the agent availabe in the alpha desktop. 
   ![Profiles](../graphics/Lab1_AI_Agent/3.47.gif)

3. Place a call to your channel. While connecting to the AI Agent, request a transfer to a human agent. Answer the call on the alpha Agent Desktop and engage in small talk about flower ordering. After disconnecting the call, the Wrap Up Summary window should appear, displaying a summary of the call between the caller and the agent.
   ![Profiles](../graphics/Lab1_AI_Agent/3.49.png)

<p style="text-align:center"><strong>Congratulations, you have officially completed this mission! 🎉🎉 </strong></p>