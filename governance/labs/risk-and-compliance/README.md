# 🧑‍💼 Managing AI Risk and Compliance with watsonx.governance

<img alt="AskHR" src="/labs/risk-and-compliance/assets/hr_landscape.jpg">




## 👋 Meet Jose – The Chief Risk Officer

Jose works at **TechCorp Inc.**, a large multinational enterprise using AI to improve HR processes like hiring and employee planning.

But there was a problem...  
AI was everywhere, but **nobody really knew**:
- Who built what
- Whether the models were fair
- If they followed rules like GDPR etc.
- What to do when something went wrong

Jose was responsible for managing all that risk — but he had **no clear way** to do it.

So, Jose and his team created decided to leverage **watsonx.governance** to make AI governance easy, clear, and reliable.


## 🎯 What Jose Wanted to Fix

Jose didn’t want to manage critical governance processes through spreadsheets, emails or slack messages. 

He wanted a simple system that would:

- ✅ **Track every AI model from start to finish**
- ✅ **Make sure models follow the rules (like GDPR, EU AI Act, etc.)**
- ✅ **Foster collaboration with the development team — without slowing them down**
- ✅ **Catch problems early and fix them fast**
- ✅ **Keep everything ready for audits**

And that’s where **watsonx.governance** helps.



## 👥 Who's involved in AI Governance?

AI Governance is a teams sport involving different roles in an organization. Though it's not uncommon to find scenarios where folks could perform the roles or severals personas, here's what these roles might look like:

<img width="854" alt="personas" src="https://github.ibm.com/skol/ai-governance-client-bootcamp/assets/12043/9294e0e5-4369-4065-8ad1-450924de45ac">


<!--
| 👤 **Role**               | 💡 **What They Can Do**                                                                 |
|--------------------------|------------------------------------------------------------------------------------------|
| **Use Case Owner**       | Create model use case, complete risk and compliance assessments, manage incident updates |
| **Stakeholders**         | Review risk levels, check compliance applicability, approve or reject use cases          |
| **Model Developer**      | Build, evaluate, and submit AI models for approval                                       |
| **Model Validator**      | Review model ethics and fairness, approve for production                                 |
| **Operations (IT/MLOps)**| Deploy approved models, monitor model performance and risks                              |
| **Risk & Compliance Officer** | Monitor risks, decide remediation actions, update stakeholders                     |

-->


## 🚀 7-Step AI Governance Implementation (Used by Jose’s Team)

A simple, structured process for managing AI models from idea to remediation.

<img alt="AskHR" src="/labs/risk-and-compliance/assets/architecture_v3.png">
<!--

### 🔹 Step 1: Create a New Model Use Case  
**Who:** Use Case Owner (Model Owner, Business Owner, Data Engineer)  
- Submit a new model use case request  
- Complete initial risk and compliance assessments  

📦 *Module: Use Case Management*

---

### 🔹 Step 2: Review Risk & Compliance  
**Who:** Stakeholders (Business Unit Leader, Head of Risk, Compliance Officer)  
- Evaluate risk level and compliance applicability  
- Approve or reject the use case  

📦 *Module: Stakeholder Review*

---

### 🔹 Step 3: Develop the Model  
**Who:** Model Developer (AI Engineer, Data Engineer, Data Scientist)  
- Build and test multiple AI models  
- Submit the best model for validation  

📦 *Module: Model Development*

---

### 🔹 Step 4: Validate the Model  
**Who:** Model Validator (Head of AI, Head of Risk)  
- Perform ethics and fairness assessments  
- Approve model for production use  

📦 *Module: Model Validation & Approval*

---

### 🔹 Step 5: Deploy the Model  
**Who:** Operations Team (Head of IT, MLOps Engineer)  
- Deploy the approved AI model to production  
- Ensure deployment is traceable to governance  

📦 *Module: Deployment Tracker*

---

### 🔹 Step 6: Monitor the Model  
**Who:** Operations & Risk Team  
- Monitor model performance and risk continuously  
- Trigger alerts and reports for anomalies  

📦 *Module: Monitor & Report*

---

### 🔹 Step 7: Manage Incidents  
**Who:** Use Case Owner & Compliance Team  
- Take remediation actions for issues and risks  
- Update stakeholders after resolution  

📦 *Module: Incident Management*

->>
---
<!--
## 🗂️ Summary Table

| ✅ **Step** | 📦 **Module**             | 👤 **Who’s Involved**         | 🧭 **What Happens**                                 |
|-------------|---------------------------|-------------------------------|-----------------------------------------------------|
| 1           | Use Case Management       | Use Case Owner                | Submit a new model use case and fill assessments    |
| 2           | Stakeholder Review        | Risk & Compliance Stakeholders| Review risk level, approve or reject the use case   |
| 3           | Model Development         | AI Engineers / Data Scientists| Build and test the AI model                         |
| 4           | Ethics Validation         | Model Validator (e.g. Head of AI) | Validate fairness, explainability, and readiness |
| 5           | Deployment Tracker        | MLOps / IT Team               | Deploy the model into production                    |
| 6           | Monitor & Report          | Operations / Risk Team        | Monitor model performance and risk metrics          |
| 7           | Incident Management       | Compliance Team & Use Case Owner | Log and remediate model-related issues         |


## 💬 What Jose Says Now

> _“Before AskHR, we had no clear process. Now everyone knows what to do, models are better, and we’re always ready for audits.”_




-->


## 🎥 Demo

(Video coming soon)


# 📄 Hands-on step-by-step lab
<img width="972" alt="Screenshot 2025-08-14 at 3 47 43 PM" src="https://github.ibm.com/skol/ai-governance-client-bootcamp/assets/12043/21836acd-f086-4e7e-99ae-be0068b4a7d7">


## ⚙️ Pre-requisites

* Access credentials (provided by the instructor)
* IBM Cloud login with assigned stakeholder role
* Services:  watsonx, OpenPages.
<!--* Instructor access to orchestration scripts-->

## 🚀 Getting Started

1. Login to [IBM Cloud](https://cloud.ibm.com)
2. Navigate to **Resource List > AI / Machine Learning**
3. Launch the **OpenPages** instance from the list.   
*If you receive an authorization error, add **/app/jspview/react/grc/dashboard/Home** to the end of the URL.*

<!--
> ![OpenPages Launch](hands_on_lab_images/cloud_openpages.png)
-->

> [!Important]
> After logging make sure to check in Profile that it has to be set as **Watsonx governance MRG Master**:

<img width="972" alt="Screenshot 2025-08-14 at 3 47 43 PM" src="https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/hands_on_lab_images/Profile.png">


> 🔐 **Note:** Make sure you're logged in as the appropriate role before proceeding with assigned tasks.



## 👩‍💼 Use Case Owner Responsibilities

<!--As a UseCase Owner, your responsibilities include:

* Creating the business and child entity
* Defining the use case (AskHR - Agentic AI)
* Submitting associated risks for approval
* Reviews submitted risks 
  
🧭 Steps:

| Step               | Action                        | Status Update                 |
| ------------------ | ----------------------------- | ----------------------------- |
| Risk Received      | Review risk description       | `Awaiting Assessment`         |
| Perform Assessment | (Optional) Add documentation  | `Awaiting Approval`           |
| Finalize Decision  | Approve / Mark Not Applicable | `Approved` / `Not Applicable` |
-->
🔍 Follow these guides:

* [Creating Business Entities](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/business_entity_creation_model_owner.md)
* [Creating and defining an AI use case](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/usecase_creation_model_owner.md)
* [Reviewing and Assessing Risk](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/risk_review_rco.md) and ensure they comply with regulatory and organizational standards.

Once the guides above have been completed, the Use Case Owner would wait for steps 2-6 in the AI Governance Implementation to be completed, in order to preceed with Step 7:
* [Mitigating Incidents](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/Mitigating_incidents.md)


💡 Don’t forget to fill in the **Risk Level** and **Control Details** before submission.


## 👤 Business Unit Leader Responsibilities

As a Business Unit Leader, you play a crucial role in stakeholder endorsement. Your input ensures the use case aligns with business strategy and acceptable risk levels.

> ⚠️ **Note:** You must be logged in as **Business Unit Leader** to access this flow.

✅ Steps to Review:

1. Go to `My Tasks` → `Stakeholder Review`
2. Open the assigned Use Case or Risk
3. Review the risk and RCO assessment
4. Leave comments (if needed)
5. Approve if compliant or reject if misaligned
6. Submit your review

🗂️ Follow this guide:

* [Stakeholder Risk Endorsement](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/risk_endorsement_BUL.md)


## 👨‍💻 Model Developer Responsibilities

As a Model Developer, your responsibilities focus on creating and evaluating Prompts and Agents for generative AI use cases. You will build and test these artifacts in the Prompt Lab and Agent Lab. Upon creation, a Factsheet is automatically generated and linked to Watsonx.governance.

You are responsible for completing any required details in the factsheet and submitting it for governance approval.

**🔐 Note:** Make sure you're logged in as Model Developer to access Prompt and Agent Labs.

🗂️ Reference:

* [Model Developer Tasks and Guidelines](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/model_developer_tasks.md)


## 🔍 Model Validator Responsibilities

As a **Model Validator**, you are responsible for monitoring and validating the AI model’s performance and fairness metrics on the **IBM Watson OpenScale** dashboard. You will review alerts related to fairness, quality, drift, and explanations to ensure the model meets governance standards.

<!--
### Key Actions:

* Log in as **Model Validator / AI Engineer**
* Navigate via **Hamburger Menu → Instances → openscale-defaultinstance**
* Open **IBM Watson OpenScale** by clicking **Open** (top right)
* Review model performance metrics for fairness, quality, and drift (focus on triggered alerts and violations; raw scores are not the primary concern)
* Evaluate the model by uploading test data provided by your instructor:

  * Click **Actions → Evaluate now**
  * Upload a CSV file containing input and expected output (ground truth)
  * Wait for evaluation to complete
* Submit feedback or observations for governance reporting

### Notes on Evaluation Dataset:

* Max size: 8 MB
* Record limits: Minimum 10, Maximum 1000
* Dataset provided by instructor
-->

🗂️ Reference:

* [Model Validator Tasks and Guidelines](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/model_validator_tasks.md)

  
## 🔍 AIOps Engineer Responsibilities

As a **AIOps Engineer**, you are responsible for Deploying the AI use case/model on **IBM Watsonx Governance** .

<!--
### 🔍  Key Actions

1. Log in to **IBM Cloud**.  
2. From the **Hamburger Menu (☰)**, navigate to **Instances → openscale-defaultinstance**.  
3. Click **Open** (top right) to access **IBM Watson OpenScale**.  
4. Review model **performance metrics** for fairness, quality, and drift.  
   - Focus on **alerts and violations**; raw scores are secondary.  
5. Evaluate the model with **test data**:  
   - Click **Actions → Evaluate Now**  
   - Upload CSV file with input features and expected output  
   - Wait for evaluation to complete  
6. Track the model and submit feedback:  
   - Click **AI Factsheet → Track in AI Use Case**

-->

🗂️ For detailed steps, refer to:

* [Operations Team Tasks and Evaluation Guide](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/Model_deployer_tasks.md)

<!--
## 📋 Summary of Stakeholder Actions

| Stakeholder Role            | Key Responsibilities                                              | Reference Guide                                                                                                                                                                                                                                                                                                                                            |
| --------------------------- | ----------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Model Owner**             | - Create business entity<br>- Define use case<br>- Submit risk    | - [Create Business Entity](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/business_entity_creation_model_owner.md)<br>- [Submit and Define Use Case](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/usecase_creation_model_owner.md) |
| **Risk Compliance Officer** | - Review and assess risk for compliance                           | - [Review and Assess Risk](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/risk_review_rco.md)                                                                                                                                                                                                   |
| **Business Unit Leader**    | - Endorse or reject risk based on alignment with strategy         | - [Stakeholder Risk Endorsement](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/risk_endorsement_BUL.md)                                                                                                                                                                                        |
| **Model Developer**         | - Create and evaluate prompts and agents for GenAI use cases      | - [Model Developer Tasks and Guidelines](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/model_developer_tasks.md)                                                                                                                                                                               |
| **Model Validator**         | - Validate model performance and fairness via OpenScale dashboard | - [Model Validator Tasks and Evaluation Guide](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/model_validator_tasks.md)                                                                                                                                                                         |
-->

## 🔍 Operations Team & Model Developer Responsibilities

As a **AIOps Engineer** or **Model Developer**, you are responsible for Managing and monitoring the AI use case/model on **IBM Watsonx Governance** .

🗂️ For detailed steps, refer to:

* [Operations Team & Model Developer Tasks and Evaluation Guide](https://github.ibm.com/skol/ai-governance-client-bootcamp/blob/main/labs/risk-and-compliance/assets/tasks/Manage_and_Monitor_Model.md)


  
## 🎉 Congratulations!

You've helped ensure this Agentic AI use case adheres to ethical AI practices by:

* Validating risk levels
* Confirming regulatory and internal compliance
* Approving only well-governed use cases
* Ensuring model fairness and quality through continuous validation

> 🛡️ Governance is not a one-time check — it’s a continuous loop of accountability and alignment.


<!--
Please find the step-by-step instructions [here](/labs/risk-and-compliance/assets/hands_on_lab_askhr_v2.md) on how you can implement this use case.
-->



