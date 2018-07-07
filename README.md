# SharePointRESTtester
A JavaScript project to use with a Content Editor Web Part to test SharePoint REST API calls. It also creates AJAX sample code and SharePoint Designer 2013 Workflow steps.

Screen captures and a detailed install can be found at: http://techtrainingnotes.blogspot.com/2017/04/a-sharepoint-rest-api-tester-with-ajax.html

Now has over 80 SharePoint REST API examples!  (see list below)

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

** Examples included **

**Search Queries (/_api/search/query)**

 - Keyword Search
 - Keyword Search with refinement filters (this one for file type)
 - Keyword Search with OR'd refinement filters (ANDs are similar)
 - People Search
 - List of all Site Collections for current user using search  (No direct REST API).
 - List of all Web Sites for current user using search  (No direct REST API).

**Misc REST Queries**

 - Get SharePoint's list of Time Zones.
 - Get Context info.

**CAML Queries**

 - CAML Query to find documents by Created date.
 - CAML Query to return all folders in a library. Uses FSObjType=1 and CAML recursive.
 
 **List items and documents**
 
 - Get a count of items in a library.
 - Get a count of items in a library. (Option #2)
 - Get all items in a list/library.
 - Get all items in a library with filename and path.
 - Get a list/library item by property and display the Title.
 - Get info about list attachments.
 - Get info about a single list attachment.
 - Get a library item by Filename and display the Title and ID.
 - Get a list/library item by ID and display the Title.
 - Get all items in a list/library filtered by date.
 - Add a new item to a list
 - Delete an item from a list using ID
 - Delete an item from a list using its URL
 - Delete an item, to the Recycle Bin, from a list using ID
 - Update an item using ID
 - Download a file.

**Folders**

 - CAML Query to return all folders in a library. Uses FSObjType=1 and CAML recursive.
 - Get a list folder's properties.
 - Get a count of items in a list folder.
 - Add a folder
 - Rename a folder

**Lists**

 - Get a list of lists from the current web. (all data)
 - Get a list of lists from the current web. (Just the title)
 - Get a list of Content Types for the current web.
 - Get a list of list columns. (Title,InternalName,FieldTypeKind,Formula,Hidden,Indexed)
 - Get a list of list columns by type. This one returns Calculated Columns.
 - Create a new list
 - Add a new folder to a list
 - Delete a list
 - Delete a list to the Recycle Bin

**Recycle Bins**

 - Get all items in web level recycle bin.
 - Get selected properties of all items in web level recycle bin.

**Site Collections**

 - Get information about the current site collection.
 - Get the size of the content in the current site collection.
 - Get the primary site collection administrator (Owner).
 - Get the primary site collection Secondary Contact.

**Webs (subsites)**

 - Get information about the current web.
 - Get the Regional Settings for the current web.
 - Get the Time Zone for the current web.
 - Get a list of all webs below the current web.
 - Get a list of all webs below the current web using "webinfos".
 - Get a web's LastItemModifiedDate
 - Create a new subsite.
 - Delete a site (Warning Will Robinson! Does not go to the Recycle Bin!)

**User Profiles**

 - Get User Profile info about the current user.
 - Get all User Profile properties for a user.
 - Get User Profile info about a user's manager. (Set "propertyName=" to any User Profile Services property.)

**Permissions**

 - Get a list of Role Definitions for a site.
 - Get a list of Site Users. The ID is useful when setting permissions.
 - Get a list of Site Groups. The ID is useful when setting permissions.
 - Get a list of Site Groups by name (filter).
 - Get info about a Site Group using the ID.
 - Get info about a Site Group using the Name.
 - Get a list of users in a Site Group.
 - Get a user by id from a Site Group.
 - Get a user by email address from a Site Group by ID.
 - Get a user by email address from a Site Group by Name.
 - Get a user by partial email address from a Site Group by Name.
 - Add a user to a Site Group by login name.
 - Remove a user from an Site Group by user ID.
 - Get a list of Site Groups where name contains 'string'.
 - Break inheritance on a subsite.
 - Break inheritance on a list.
 - Break inheritance on a list item.
 - Grant permissions (Role Assignment) on a list.
 - Remove permissions (Role Assignment) on a list.

**Filter Select and OrderBy**

 - Get a list of Site Users who are not Site Collection admins. Get selected fields and sort.

**SharePoint 2010 style REST - _vti_bin/ListData.svc**

 - Get a list of lists and libraries (EntitySets).
 - Find list items greater than a date.
 - Find list items between two dates.
