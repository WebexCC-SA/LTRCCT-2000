---
#icon: material/folder-open-outline
icon: material/medal
---



# Mission 3: Configure Fulfilment Action and create an order.

 **<details><summary>What is Transfer to Webex AI Agent Action? <span style="color: orange;"></span></summary>**



Transfer Action is a task that an AI agent performs by understanding user intents and transferring the interaction back to the WxCC flow with custom data for further processing.



</details>
---


## Mission overview
Your mission is to:

For this mission, the proctor has created Webex AI Agent named **Flower_Wholesale**. The goal of this mission is to transfer the call from your AI agent to **Flower_Wholesale** using the Transfer operation.
   ![Profiles](../graphics/Lab1_AI_Agent/TransfertoAI.png)

---

## Build

### Task 1. Create Transfer to flow action in AI Agent Studio portal. 

1. Open your AI agent with name **<copy><w class="attendee"></w>_2000_AutoAI_Lab</copy>** and then click on **Actions**.Action**. 
    ![Profiles](../graphics/Lab1_AI_Agent/14.1.png)

2. Select **Transfer_to_different_department** action. 
    ![Profiles](../graphics/Lab1_AI_Agent/14.2.png)

3. Adjust the Transfer condition by adding **or Wholesale** as the department option. 
    ![Profiles](../graphics/Lab1_AI_Agent/14.3.gif)

4. Adjust entiry example by adding **Wholesale**. 
    ![Profiles](../graphics/Lab1_AI_Agent/14.4.gif)

5. **Save** and **Publish** the changies. 
    ![Profiles](../graphics/Lab1_AI_Agent/14.5.gif)