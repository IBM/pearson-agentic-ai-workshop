# Instructions for instructor setup

## 🍃 Environment Setup

1. Create a [Techzone Reservation](https://techzone.ibm.com/my/reservations/create/68937a8265308ff2531b7c63).  This can take several hours to provision. 

   <img src="./gov-environment-tz.png" width=50% height=50%>

> [!NOTE]  
> You should only need one reservation and then provide access to the students.  This will allow them to share an environment and see the shared work in labs where that is highlighted. 

2. When you are invited to the environment, you'll receive an email. This message is from IBM Cloud (no-reply@cloud.ibm.com) inviting you to join the account where your environment is located. In the email, look for words **Join Now** (Highlighted in the screenshot below.)
   
   <img src="./techzone.png" width=75% height=75%>


## Configuration
### OpenScale
Navigate to [OpenScale](https://aiopenscale.cloud.ibm.com/aiopenscale/insights?nocache=true) (making sure you are in the correct cloud account) and ensure it is configured and has a database. 

1. The auto setup dialog should be visible. Click on Auto setup to configure OpenScale. This process can take around 30 minutes.  

<img src="./openscale-auto-config.png" width=75% height=75%>

> [!NOTE]  
>If there is an error, you can use the Manual setup option and pick the defaults.

2. Click on the Let's go button.

 <img src="./openscale-lets-go.png" width=75% height=75%>

> [!NOTE]  
>If you do not see the Auto Setup dialog, ensure you are in the right cloud account by clicking the User icon in the top right and selecting the cloud account from the drop down. Click the User icon to close the side panel.

<img src="./openscale-user-account.png" width=50% height=50%>


You can click on the configuration button on the left menu to confirm the setup.

<img src="./openscale-config.png" width=75% height=75%>

  
<img src="./openscale-configured.png" width=75% height=75%>

### watsonx.gov

Open the menu from the top left and pick **Inventories**

<img src="./ai-inventory.png" width=40% height=40%>  

then click on the **Complete Setup** button

<img src="./gov-setup1.png" width=75% height=75%>

and choose the COS from the drop down, and click **Create** to complete the setup.

<img src="./gov-cos-create.png" width=75% height=75%>

> [!IMPORTANT]  
>If you get an error stating that the default inventory could NOT be created, try following the troubleshooting steps listed in [this guide](./default_inventory_issue.md).  
>  <img src="./setup-error.png" width=50% height=50%>

After the default inventory is created, add access to the inventory by clicking on the 3 dots and then clicking on **Set collaborators**  
<img src="./inv_collab1.png" width=75% height=75%>

Then choose **Add Collaborators** and choose **Add user groups**  
<img src="./inv_collab2.png" width=50% height=50%>

Then, you can search on the access group - the environment contains one that starts with **eid** that you can add.  Instructors should be added to this Access Group.  You can also add to this by using the **Add users** button and adding instructors/students as required.    

<img src="./inv_collab3.png" width=50% height=50%>

## Create an API key

To create an API Key, go to [IBM Cloud](https://cloud.ibm.com/) encuring that you are in the correct account (as you did above)

1. Click on the **Manage** menu, and then **Access (IAM)**  
<img src="./iam-access.png" width=75% height=75%>

2. Click on **API Keys** on the left menu, then click **Create** to generate a new API key.  
<img src="./api-key.png" width=75% height=75%>

3. Enter a name and click **Create**  
<img src="./api-key-create.png" width=75% height=75%>

4. Copy or download the API key. You will not be able to see it again, so it's important to save it at this point and copy it somewhere you can get to it!  
<img src="./api-key-copy.png" width=75% height=75%>


## Create an Evaluator for Metrics

During the process of running through the [Automatic Evaluation](../../labs/monitoring-and-guardrails/automatic-eval.md) exercise you will be prompted to [Configure Evaluation Metrics](../../labs/monitoring-and-guardrails/automatic-eval.md#-configure-evaluation-metrics).  Instuctions are in-line for creating an LLM judge, but this can be done before the bootcamp by running through this lab ahead of time. Once the evaluator is added it will be available for others to use. 

**Step 1:** Adding Evaluator to have an LLM judge

You can configure settings to calculate metrics with LLM-as-a-judge models. LLM-as-a-judge models are LLM models that you can use to evaluate the performance of other models.

To calculate metrics with LLM-as-a-judge models, you must select Manage to add a generative_ai_evaluator system when you configure your evaluation settings.

LLM as Judge [documentation](https://dataplatform.cloud.ibm.com/docs/content/wsj/model/wos-monitor-gen-quality.html?context=wx&audience=wdp&locale=en)


Select the **Add** button in the new window and then continue to give it a name, add your API key created from before, and choose a model:

   <img src="./llm-as-judge.png" width=75% height=75%>
   <img src="./api-addition.png" width=75% height=75%>

These instructions are included in the lab as well, but the instructor should normally do this before running the bootcamp so students can pick the existing evaluator. 

## Share the Reservation

Share the reservations with your attendeees, by clicking on the top right of the [reservation](https://techzone.ibm.com/my/reservations) and pick Share.  

   <img src="./tz-share.png" width=50% height=50%>

Then add the emails of the attendees, with a semi-colon as a separator

   <img src="./tz-share-email.png" width=75% height=75%>

Alternatively you can add people to the cloud environment using IAM by clicking on **Manage** on the top bar, and select **Access (IAM)** and add adding the users.

In both cases, they will get an email notifying them that they have been added to the cloud account. 

<img src="./cloud-iam.png" width=75% height=75%>


