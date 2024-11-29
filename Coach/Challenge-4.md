# Challenge 4 - Coaches Guide

## RAG Pattern

## Task - 01

1. Login to the Azure AI portal at `https://ai.azure.com/`.
   
2. Click on **create project** , Give an unique name to the project.

   ![newdatasource](images/create-project-1.png)

3. Under Create a project.
    - Project name : Unique name
    - Hub name : Provide an unique name.

   Then click on create
   

5. On the **Create a hub** pane , Provide the details as shown below:
   
    - Hub name : Leave as default
    - Subscription : Leave as default.
    - Resource Group : choose **OpenHack** from the drop down.
    - Location : Leave default.
    - Connect Azure AI services : Leave default.

    ![newdatasource](images/create_hub00.png)
    
7. Select create new AI search , A new browser page will open , log in using your credentials.
   
     - Resource Group : Openhack
     - Service name : Give a unique name.
     - Location : **East US**.
     - Pricing tier : Choose standard.
     - Click on **Review + Create** and proceed with the creation.
   
    ![newdatasource](images/search-01.png)
    
    ![newdatasource](images/search-create.png)

8. Under "My Assets," select **Models + Endpoints**, then click on **Deploy a Model** and choose **Deploy a Base Model**.
    
    ![newdatasource](images/model+endpoints.png)

9. Choose gpt-4o and click on confirm.

    ![newdatasource](images/gpt-4o.png)

10. Fill in the details as shown below:
    
    - Deployment name : Gpt-4o
    - Deployment type : Global Standard
    - Click on customize
    - Token's per Minute rate limit : 10k

     ![newdatasource](images/deploy-1.png)
     
11. Click on **Playground** and then select **Try the Chat Playground** .
     
    ![newdatasource](images/playgrounds.png)
   
1. Click on the **Add your data** tab and then click **Add new data source**  
    
    ![newdatasource](images/add-data.png)
    
1. On the **Data source** dropdown choose **Upload files**

    ![uploadfiles](images/uploadfiles-1.png)

1. From the **Upload** button click the arrow and select **Upload files**

    ![uploadfiules 2](images/uploadfiules2-1.png)
    
1. Click on the **Next** button

    ![next 1](images/pdf.png)
    
1. After deployment return back to the **Azure AI Studio**and from the dropdown select **Connect other Azure AI Search resource**

    ![other](images/connect-ai.png)
    
1. Click **Add connection**

    ![addconnection](images/add-connection.png)

1. Create a indentifiable **Index name** and click **Next**

    ![indexname](images/search.png)
    
1. Leave the default settings on the **Search settings** page. Click **Next**

    ![settings](images/search-2.png)

1. Click **Create vector index**

    ![settings](images/create-vector.png)

1. Give it some time to **Crack and chunk** the data

    ![crack](images/chunk.png)

1. Once completed change the **Search** type to **Hybrid(vector + keyword)**

    ![hyrid](images/hackvector.png)
    
1. Expand the **Advanced settings** section and max out the following:

    ![advanced](images/-1.png)
    
1. Use the following prompt

    ```
    Which A_Category has the most returns?
    ```
1. Results...

    ![rag 2](images/rag2-1.png)
    
    > Note: There might be issues getting it to complete correctly with the following kinds of errors provided. Seems like repeating the prompt and selecting different **Search type(s)** works most of the time. Also refreshing the page and selecting the index resolves the issue too.

    ![errors](images/errors-1.png)

    > Another possible answer result
    
    ![answer 2](images/answer2-1.png)

## Bonus
- Using the System message map the A_Category to the word Category to make the prompt easier to use.
