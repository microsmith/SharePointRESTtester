# SharePointRESTtester
A JavaScript project to use with a Content Editor Web Part to test SharePoint REST API calls and create AJAX sample code and SharePoint Designer 2013 Workflow steps.

Screen captures and a detailed install can be found at: http://techtrainingnotes.blogspot.com/2017/04/a-sharepoint-rest-api-tester-with-ajax.html


To use:
---------

 1. If your master page is not already loading jQuery, download jQuery (just about any version) and upload to the Site Pages library.
 2. Download the SharePointRESTtester.html file to your PC.
 3. Edit the file and update the line that loads jQuery to point your jQuery file. If your master page already loads jQuery, then delete the &lt;script&gt; block that loads the jQuery file. (the first line of the file)
 4. Upload the SharePointRESTtester.html file to your Site Pages library. (Copy the URL to the file.)
 5. Add a Web Part Page to your project:
 5.1 In the Site Pages library, click the **FILES** ribbon, click **New Document** and click Web **Part Page**.
 5.2 Enter a page name like "SharePointRESTtester".
 5.3 From the library dropdown select **Site Pages**.
 5.4 Click Create.
 6. Click **Add a Web Part**.
 7. Add a Content Editor Web Part.
 8. Click the web part's dropdown and click **Edit Web Part**.
 9. Enter or paste the path to the SharePointRESTtester.html file. 
 10. Click **OK** and then in the ribbon click **Stop Editing**.
 11. You should now see the tester. Click the dropdown and you should see data in the boxes. If not, then the jQuery library did not get loaded.

