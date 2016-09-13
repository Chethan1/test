 Marketo Webhooks

Marketo allows the use of Webhooks to communicate with third party web services. Webhooks support the use of the GET or POST HTTP verbs to push or retrieve data from a specific URL.

Step1 : Create a webhook

1)Log in to marketo 

2)Go to admin->webhooks



![image2014-9-24 14_52_57](https://cloud.githubusercontent.com/assets/11537436/18479556/15ed34b4-79f3-11e6-9b32-7843c98f0a9d.png)

3)Click on new webhook

![image2014-9-24 14_53_9](https://cloud.githubusercontent.com/assets/11537436/18479563/17b8841a-79f3-11e6-8739-305c8ecd9d45.png)

3) Name and configure your webhook.

![image2014-9-24 14_53_19](https://cloud.githubusercontent.com/assets/11537436/18479565/18c1945a-79f3-11e6-9247-cf8369c9d590.png)



    URL: Enter the URL you use to POST your request to the web service. To insert a token, such as the lead's email address ({{lead.Email Address}}), in your request, click Insert Token.
    Template: If you wish to transmit information in the body of the POST, enter the template. Use any data format that supports HTTP POST, including XML, JSON, or SOAP. To insert a token in your template, click Insert Token.
    Request Token Encoding: If the token values include special characters (such as an ampersand, '&'), indicate the format of your request (JSON or Form/Url).
    Response type: Select the format of the response you receive from the service (JSON or XML).


4) Click Create.



![image2014-9-24 14_53_35](https://cloud.githubusercontent.com/assets/11537436/18479567/19bfbfda-79f3-11e6-9dac-6d9bd9f4c157.png)

Step 2: Triggring a webhook

1)Go to Home and then My Marketin Activities

![marketing](https://cloud.githubusercontent.com/assets/11537436/18481492/fe62c190-79f9-11e6-98e9-e078be7a2f36.png)

2)Go to Marketing activities-> New ->New Smart Campaign


![screen shot 2016-09-13 at 9 42 39 pm](https://cloud.githubusercontent.com/assets/11537436/18481770/17480c32-79fb-11e6-884e-13117d24d6f4.png)

 
 --Folder : Enter the smart campign folder name under which you want to create the smart campaign.
  
  --Name: Name of the new campaign.
  
   Click on create
  
 

 

![screen shot 2016-09-13 at 9 47 07 pm](https://cloud.githubusercontent.com/assets/11537436/18481905/b57424e0-79fb-11e6-9183-274a732a88b1.png)

3)Go to smartlist-> Go to the list of trigger on your righthand side drag and drop Lead is Created


![screen shot 2016-09-13 at 9 55 50 pm](https://cloud.githubusercontent.com/assets/11537436/18482214/e0299e76-79fc-11e6-8b2a-d8c5d38d48a1.png)


4)Go to Flow->Under integration drag and drop the Call Webhook-> select the webhook that you have created in the first step.


![image2014-9-22 15_8_2](https://cloud.githubusercontent.com/assets/11537436/18479541/09ac7336-79f3-11e6-94d8-505921e381a9.png)


![image2014-9-22 15_8_5](https://cloud.githubusercontent.com/assets/11537436/18479548/0fd5d298-79f3-11e6-99ac-03b295fe7f82.png)

5)Go to shedule click on Activate.

![screen shot 2016-09-13 at 10 02 20 pm](https://cloud.githubusercontent.com/assets/11537436/18482462/d436bcba-79fd-11e6-8a88-ab1a84ef5b73.png)


Step 3:Testing a webhook
	
	Create a New Lead in marketo.



Step 4:To check the results.
	go to Go to Marketing activities->go to New smart Campaign you have created->go to the results section you will be able to the status of the webhook whether it has triggered or not.


![reult](https://cloud.githubusercontent.com/assets/11537436/18482547/313aee54-79fe-11e6-8022-540746fd8366.png)
	
	



