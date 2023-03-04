![Hackathon Logo](docs/images/hackathon.png?raw=true "Hackathon Logo")
# Sitecore Hackathon 2023

- MUST READ: **[Submission requirements](SUBMISSION_REQUIREMENTS.md)**
- [Entry form template](ENTRYFORM.md)
  
### ⟹ [Insert your documentation here](ENTRYFORM.md) <<
# Team
Team Horizon 2023

# Category
1.	Best Enhancement to XM Cloud

# Our Solution Summary

- Latest Sitecore 10.3 and XM Cloud introduced a new management and administration APIs and webhooks capabilities. Our hackathon idea is to develop best enhancement to XM Cloud leveraging the new webhooks capabilities. Our fictitious global marketing company, Horizon has faced challenges managing the transcreation of our global content to all our markets. 
- Globa, our global content producer needs to assign content transcreation orders efficiently, notify her team to action, translate content to various localized languages to meet our business needs. 
- Nicola, the localization specialist needs to leverage modern AI tooling to help with transcreation process efficiently to meet tight deadlines. 
- Rupet, our reporting guru loves visibility and wants to communicate with global campaign managers on transcreation orders. 
- Brenda, our marketing brand manager wants content available to omni-channels for all locales to meet global demands.

# Solution Design

1.	We leverage the Sitecore XM webhooks functionality to trigger transcreation work orders raised by Globa, our global content producer. She does this by creating new versions, in Sitecore XM, of content for different languages to meet global needs.  
2.	Our Notifications Hub will process the webhooks from Sitecore XM using Serverless Functions hosted on our managed Azure cloud. This will push direct messages and notifications to our team of transcreation analysts, lead by Nicola. 
3.	It also logs all transcreation orders in Cosmos DB repository, which acts as store tracking changes done during transcreation processes and content strategy workflows. 
4.	We have a JamStack web portal which Nicola and her team will use to pick the logged transcreation orders, proces them through agreed workflows. 
5.	We leverage the Open AI API integration to efficiently localize and translate content as per the requests. All approved content will then be fed back into Sitecore XM Cloud using the REST APIs 
6.	Brenda will then work with Globa to review the final content in XM Cloud, publish this to a global CDN (Sitecore Delivery Platform) to meet the omni-channel needs for our business

<img width="1507" alt="Sitecore Hackathon-2023 - Team Horizon 2023" src="https://user-images.githubusercontent.com/48400867/222894599-fcc2e6ac-6eb4-4e10-9102-a224a8e094b5.png">


## Video link
⟹ Provide a video highlighing your Hackathon module submission and provide a link to the video. You can use any video hosting, file share or even upload the video to this repository. _Just remember to update the link below_

⟹ [Replace this Video link](#video-link)



## Pre-requisites and Dependencies

⟹ Does your module rely on other Sitecore modules or frameworks?

- Sitecore XM 10.3 with Webhook configuration
- We are using Azure Function App as Notification Hub
- Azure Cosmos DB as a repository to track our transcreation work orders
- JamStack web portal to pick the transcreation orders
- Open AI integration to translate the content


## Installation instructions
⟹ Write a short clear step-wise instruction on how to install your module.  

1. Globa created content in Sitecore content Editor in English (en-US), webhook triggered our notification Hub.Below is the screenshot where is processing the item
3. Function App sent the email notification to Nicola the localization analyst
4. It also logged the data in Cosmos DB
5. We have integrated with OpenAI API which translates the content as per the request

## Usage instructions
⟹ Provide documentation about your module, how do the users use your module, where are things located, what do the icons mean, are there any secret shortcuts etc.

Include screenshots where necessary. You can add images to the `./images` folder and then link to them from your documentation:

![Hackathon Logo](docs/images/hackathon.png?raw=true "Hackathon Logo")

You can embed images of different formats too:

![Deal With It](docs/images/deal-with-it.gif?raw=true "Deal With It")

And you can embed external images too:

![Random](https://thiscatdoesnotexist.com/)

## Comments
If you'd like to make additional comments that is important for your module entry
