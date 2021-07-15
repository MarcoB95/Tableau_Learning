# Tableau Fundamentals

## Connect to and Customize Data

### Connecting to data

Live connections vs. extracts:

- Connecting live, which is the default connection, leaves the data in the database or source file. This is best when you want to leverage a high performance database’s capabilities, or to get up-to-the-second changes in data visualized in Tableau

- You can alternatively choose to extract the data into Tableau's high performance in-memory data engine. This option is useful when you connect to a slow database or when you want to take query load off critical systems

The types of flat files you can connect to include Microsoft Excel files, text files, JSON files, PDF files, and more. Once you've connected to a data source, Tableau opens to a workbook with the data loaded. This is the Data Source page. Metadata describes your data. It includes the names of fields and data types as well as aggregation information and default display properties. Tableau assigns metadata to the data that you bring into Tableau; you can edit the metadata in a way that better supports how you want the fields to look and function when you're building a view. If you need to reference something quickly or wish to see some of the name changes that you've made, click the Manage metadata button to switch to the metadata grid view. The metadata grid displays the fields in your data source as rows so that you can quickly examine the structure of your Tableau data source and perform routine management tasks, such as renaming fields or hiding multiple fields at once.

### Customizing a Data Source

When analyzing data, you may need to do some cleanup and organization as you work with the underlying source data. This could include customizations like connection information, organizational or metadata changes, attributes, or aliases. Note that Tableau preserves the customizations you make, but it does not change the underlying source data.

Tableau automatically predicts whether your fields are dimensions or measures, but sometimes you may want to re-categorize a dimension as a measure or vice versa. To make the field names more intuitive, Tableau allows you to rename any of the database fields. To clarify the meaning of the labels associated with discrete dimension members in the view, Tableau allows you to create aliases, or alternate names. You can edit a field’s default properties, such as color, number format, or aggregation. This way, every time you add the field to the view, it will maintain its assigned properties.

## Organize Data and Create Filters

### Creating Groups in Your Data

A group lets you combine several members of a single dimension into a single data point or category type, creating a new dimension field that didn’t originally exist in your data (Groups in Tableau are represented by a paper clip). Groups can be created using each of the following methods:

- Create a group based on a field in the Data pane
- Create a group based on labels in the view
- Create a group based on marks in the view

Once a group as been created within the Create Group dialog, you can check Include 'Other' to group all remaining members into a group. The group will be assigned the name Other and can be renamed as needed.