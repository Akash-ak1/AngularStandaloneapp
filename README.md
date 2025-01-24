Task Description: File Upload and Search Functionality
Objective:

We need to build a comprehensive feature where users can upload Excel files, view and filter the data, and then download the results in an Excel file format. The solution should be built using Angular (latest version), .NET Core, and SQL Server.

1. UI for File Upload in Angular
Functionality:

Users will be able to browse and select an Excel file from their system using a file input element.

Once a file is selected, the file will be uploaded to the server.

After the upload, the system will parse the Excel file and insert the data into the SQL Server database.

Requirements:

A file input component to select the Excel file.

A button to trigger the upload process.

Display appropriate success/error messages based on the upload status.

2. UI for Search Screen with Filters
Functionality:

The search screen should display the data from the database, with certain columns highlighted in yellow for filtering.

Users can enter values in the filter inputs (for the highlighted columns) and click on the "Search" button to retrieve filtered results from the database.

The system should dynamically filter and display data based on the entered values.

Requirements:

Display a grid/table of the data with options for filtering based on certain columns (highlighted in yellow).

Input fields for each filterable column.

A button to trigger the search functionality, which will query the database and display the results.

3. Downloadable Search Results in Excel Format
Functionality:

After performing the search, users should be able to download the displayed results in an Excel file format.

Requirements:

A "Download" button to trigger the download functionality.

The data displayed on the UI should be converted into an Excel file and made available for download.

Test Cases
Test Case 1: File Upload

Steps:

Navigate to the file upload screen.

Browse and select an Excel file.

Click on the "Upload" button.

Verify that the file is uploaded successfully.

Expected Result: The data from the Excel file should be inserted into the SQL Server database.

Test Case 2: Search with Filters

Steps:

Navigate to the search screen.

Enter values in the filter fields corresponding to the yellow-highlighted columns.

Click on the "Search" button.

Expected Result: The search results should be displayed based on the entered filter criteria.

Test Case 3: Download Search Results in Excel

Steps:

Perform a search to display results.

Click on the "Download" button.

Expected Result: The search results should be converted into an Excel file and be available for download.

Test Case 4: Invalid File Upload

Steps:

Navigate to the file upload screen.

Browse and select an invalid file (non-Excel file).

Click on the "Upload" button.

Expected Result: An error message should appear indicating that the selected file is not a valid Excel file.

Test Case 5: No Results Found for Search

Steps:

Navigate to the search screen.

Enter filter values that do not match any records in the database.

Click on the "Search" button.

Expected Result: The UI should display a message indicating "No results found."

Requirements Document
System Overview:

File Upload Screen:
      - Users can upload an Excel file through a file input component.
      - The system will parse the Excel file and insert the data into the SQL Server database.
      - After a successful upload, a success message will be displayed. If there is an error (e.g., invalid file format), an error message will be shown.

   Search Screen:
      - The UI will display a table/grid of data fetched from the database.
      - Some columns will have filters that users can use to search and filter data.
      - Upon entering filter values and clicking the "Search" button, the system will query the database and display the filtered results.

      Download Feature:
      After performing a search, users can download the filtered results as an Excel file.

   Non-Functional Requirements:

   Performance:
       The system should efficiently handle large Excel files and data results without significant delays.

      Usability:
       The UI should be user-friendly with clear instructions for uploading files, searching, and downloading results.

      Compatibility:
      The application should be compatible with modern browsers.

      Security:
   Only valid Excel files should be uploaded to prevent security vulnerabilities.

      Scalability:
      The system should be scalable to accommodate increasing data volume in the future
