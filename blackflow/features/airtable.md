---
description: These are the essential part of the airtable documentation
---

# 🤓 Intro to airtable

## What's a base?

[Main points](https://support.airtable.com/hc/en-us/articles/360021518753#h_3fbdd22f-101f-4515-b88d-a6c0f433a3c5)

* A [**base**](https://support.airtable.com/hc/en-us/articles/360021518753#base) is a database that contains all of the information you need for a specific project, and is made up of one or more tables.
* Each base is made up of one or more **tables**. A [**table**](https://support.airtable.com/hc/en-us/articles/360021333094#table) contains a list of items of the same type—like people, ideas, or projects.
* Each table is comprised of records and fields. By default, a table looks like a grid, with records as the rows and fields as the columns.
* A [**record**](https://support.airtable.com/hc/en-us/articles/360021333094#record) is an individual item in a table.
* Information related to each record is stored in rich [**fields**](https://support.airtable.com/hc/en-us/articles/360021333094#field). Each field can store a different type of information, like text, checkboxes, file attachments, ratings, select options, and more.
* You can change a field's type and adjust its formatting with the [**field customization menu**](https://support.airtable.com/hc/en-us/articles/360021333094#new-field).
* You can [**expand a record**](https://support.airtable.com/hc/en-us/articles/360021333094#expanded) to see all its associated details in a card-like layout.

![](../../.gitbook/assets/image%20%282%29.png)

## [What's a table?](https://support.airtable.com/hc/en-us/articles/360021333094#table) <a id="table"></a>

A **table** contains a list of items of the same type—like people, ideas, or objects. Each base needs at least one table, and if your base is tracking different types of items, it'll probably make sense to divide your base into multiple tables. For example, a base for a sales pipeline could have separate tables for sales leads, companies, and deal opportunities, whereas a base for planning a wedding could have separate tables for potential venues, attendees, and wedding registry items.

Toward the top of your base, you'll see a tab that says "Table 1." Our new base starts out with just this one table. Eventually, we might want to add more tables to our base, but for now, let's just rename Table 1 to "Artists." This table is where we'll put all the information that we want to track for the artists.

![rename-table.gif](https://support.airtable.com/hc/article_attachments/360031381234/rename-table.gif)

## [What's a record?](https://support.airtable.com/hc/en-us/articles/360021333094#record) <a id="record"></a>

Each row that you see in the grid is called a **record**. A record is an individual item in a table and could be many different things: for example, if you're making a table of tasks that need to be completed, then each row in your table is a task; if you're brainstorming a list of new ideas, then each row in your table is a new idea.

Since this is our Artists table, each record in in the table is going to be a different artist that we want to store information about. Let's go ahead and fill in the names of three artists in the first column \(the one that says “Name” at the top\).

![add-new-records-10fps.gif](https://support.airtable.com/hc/article_attachments/360031381354/add-new-records-10fps.gif)

Additionally, you can also select any cell and use the keyboard shortcut Shift + Enter to insert a new record below the selected cell. Now, using whatever methods you want, go ahead and add some more records to this table.

## [What's a field?](https://support.airtable.com/hc/en-us/articles/360021333094#field) <a id="field"></a>

These columns are called **fields**, and they give you a structure in which you can put the details that are relevant to each record.

Each field has a special **field type** that determines what kind of rich information you can put in it, like long text notes, drag and drop file attachments, checkboxes, dropdown select options, and more. By picking and choosing the correct field types, you can make a base that's custom-fit for your unique needs!

The Notes field is a long text field, which is good for holding multiple lines of text.

![long\_text.gif](https://support.airtable.com/hc/article_attachments/360032352633/long_text.gif)

The Attachments field lets you upload one or more files to individual records, including ad image. You can drag and drop files into the individual cells, or you can click on the gray plus sign button that appears when you click into a cell to bring up an image upload dialog.

![drag\_and\_drop.gif](https://support.airtable.com/hc/article_attachments/360033094213/drag_and_drop.gif)

After filling out your first three fields, your table should look something like this:

Feel free to download this CSV to use yourself, or directly copy and paste the cells in this embedded table and paste them into your own base.



## What's a view? <a id="h_d39ff82d-a4e0-4c6f-9c40-a94802be8650"></a>

Main points

* [**Views**](https://support.airtable.com/hc/en-us/articles/360021501754#what-are-views) let you customize how information is displayed in a table: all the underlying information is the same, but how and what is shown can differ.
* [**Filters**](https://support.airtable.com/hc/en-us/articles/360021501754#filters) allow you to hide certain records from a view depending on values in their fields.
* You can also choose to show or [**hide**](https://support.airtable.com/hc/en-us/articles/360021501754#hide) specific fields, which allows you to focus on a smaller subset of relevant fields without changing or deleting any of the underlying data.
* The order in which records appear is also specific to a view. You can manually rearrange records, or you can apply a [**sort**](https://support.airtable.com/hc/en-us/articles/360021501754#sort) so that your records appear in a particular order according to the values in specific fields.
* You can make as many views as you'd like and [switch back and forth between them](https://support.airtable.com/hc/en-us/articles/360021501754#switch) depending on what you want to see, when.



#### **Making a new view**

Whenever you look at your information in Airtable, you're _always_ looking at it through a view. The default view you get when you make a base from scratch is a grid view with no hidden fields, filtered records, or specific sorting called "Grid view."



![new-grid-view.gif](https://support.airtable.com/hc/article_attachments/360032713533/new-grid-view.gif)

#### **Filters**

One of the core features of [views](https://support.airtable.com/hc/en-us/articles/202624989) is the ability to filter records according to particular criteria. When a record is filtered, it is _not_ deleted—it's just hidden from the particular view you're using to look at your table. Filters are a great way to hide inactive records or [archive them](https://support.airtable.com/hc/en-us/articles/360013686833) if you don't need them anymore—without permanently deleting any historical information in case you need it later. Let's use filters to hide any of the artists that aren't currently active.  
  
Click on the filter button in the view bar to bring up the filter menu. As you might expect, you'll see a notice indicating "No filters applied to this view."

![no-filter.png](https://support.airtable.com/hc/article_attachments/360031893754/no-filter.png)

Go ahead and click the + Add filter button. This will create a new filter condition that you can customize. First, let's set the filter field. Right now it says "Name," but since we want to filter records based on the values in the Status field instead, let's click on the dropdown and pick Status.

![filter-field.jpg](https://support.airtable.com/hc/article_attachments/360031893894/filter-field.jpg)

Lastly, we need to select the comparison value, which is the value that you'll be comparing your records to. If you click on the Select an option dropdown, you'll get a selection menu much like the one you see when picking a cell value in a single select field. Let's pick Active, to make the filter condition complete: we want to see records where **Status** **is** **Active**.

![active-filter.gif](https://support.airtable.com/hc/article_attachments/360031894074/active-filter.gif)

### [Hiding fields](https://support.airtable.com/hc/en-us/articles/360021501754#hide)

Filters hide records \(rows\), but you can also choose to hide certain fields \(columns\) from a view. To control the visibility of the fields in your view, click on the Hide fields button in the view bar.

![hide-field.png](https://support.airtable.com/hc/article_attachments/360031995274/hide-field.png)



### [Sorting](https://support.airtable.com/hc/en-us/articles/360021501754#sort)

The order in which records appear is specific to a view \(unlike a spreadsheet, in which the number of a row is an inherent property of the row\). This means that different team members can easily rearrange records within a view to look at them in whatever way is most convenient for the task at hand, without affecting the order of records in other views.

#### Manually reordering records

You can manually reorder rows by clicking on the drag handle that appears when you mouse over a record, then dragging the row to a new location.

![manual-sort.gif](https://support.airtable.com/hc/article_attachments/360032840333/manual-sort.gif)

You can also select a range of rows to move by clicking on the checkbox that appears when you mouse over a record, holding the Shift key, and then clicking on the last record number in the range you want to select.

#### Automatically sorting records

You can also apply one or more sorts to your view that will automatically arrange your records in a particular order according to the values in specific fields. To apply a sort to your view, click the sort button in the view bar. Since we don't currently have any sorts applied, the sort menu will say "No sorts applied to this view." Let's sort our artists by how soon their contracts are expiring. Create a new sort by clicking on the Pick a field to sort by dropdown, then selecting the Contract End field.

![automatic-sort.jpg](https://support.airtable.com/hc/article_attachments/360032024154/automatic-sort.jpg)

Records will now automatically sort themselves in this view if any changes occur to records that would cause them to be ordered differently. The sort button will get a soft orange highlight, as will any visible fields being used for sorting criteria. When automatically sorting records, you won't be able to manually rearrange records.

If you'd prefer, you can switch off the Keep sorted toggle. This will allow you to sort records only when you decide to apply the sort using the Apply sort button

### Switching between views

We've now finished setting up our own custom view that shows just the currently active artists on our roster, and stays automatically sorted to show which contracts will be ending soonest. At any time, we can switch from this view to see another view.

To switch between your existing views, click on the dropdown arrow next to the name of the view. From the view switcher, you can see all of the views associated with this table. Right now, you should only have two—All Artists and Currently Active. Click on All Artists to switch back to the original view.

![view-switch.gif](https://support.airtable.com/hc/article_attachments/360032847333/view-switch.gif)

## View Type

Main points

* The default view type is [**grid view**](https://support.airtable.com/hc/en-us/articles/360021502314#h_612e470a-cbba-4796-bf18-9d6ccc9c9938), which displays a grid with your records as rows and your fields as columns. Each table must have at least one grid view.
* Grid views have a number of special features, like [**grouped records**](https://support.airtable.com/knowledge/articles/360021502314/en-us?brand_id=238265#h_2b17969d-9ba9-470d-87d8-30dbfca4b47c) and the [**summary bar**](https://support.airtable.com/knowledge/articles/360021502314/en-us?brand_id=238265#h_45af5a7a-b7f2-4e77-bfe2-29aaa7b61138).
* [**Calendar view**](https://support.airtable.com/knowledge/articles/360021502314/en-us?brand_id=238265#h_09de72bb-b976-4ee9-b55b-fb382448dc41) displays your records as events on a calendar. Your table must have at least one date field in order to make a calendar view.
* [**Kanban view**](https://support.airtable.com/knowledge/articles/360021502314/en-us?brand_id=238265#h_fe5caf18-e280-4097-8a45-fd11216974b6) displays your records as cards on a kanban board. Your table must have at least one single select field or single collaborator field in order to make a kanban view.
* [**Gallery view**](https://support.airtable.com/knowledge/articles/360021502314/en-us?brand_id=238265#h_610b99ad-8481-432d-a95a-90050d1c1f23) displays your records as large cards and is particularly good for showing off images.
* [**Forms**](https://support.airtable.com/knowledge/articles/360021502314/en-us?brand_id=238265#h_3579a188-40d6-4698-bc63-8515e29acc4a) can also be created from the view bar and are used to add new records to your table.

##  <a id="h_612e470a-cbba-4796-bf18-9d6ccc9c9938"></a>

### [Grouped records](https://support.airtable.com/hc/en-us/articles/360021502314#h_2b17969d-9ba9-470d-87d8-30dbfca4b47c) <a id="h_2b17969d-9ba9-470d-87d8-30dbfca4b47c"></a>

In a grid view, you can group records together based on their shared values in one or more fields. It's a great way to make quick visual distinctions between the different records in your table. Go ahead and click the group records button in the view bar to bring up the grouped records menu.  
  
You'll see a notice indicating "No groupings applied to this view." Go ahead and click the Pick a field to group by dropdown, then select the Status single select field. This will split our artist roster into different groups based on the values in the Status field.  
  
  
  
You can change the values for a record by dragging it from one group to another group. Try dragging one of the records from one group to another—the value in the Status field will automatically change accordingly.

![how-to-group.gif](https://support.airtable.com/hc/article_attachments/360032025694/how-to-group.gif)

![drag-her.gif](https://support.airtable.com/hc/article_attachments/360032025774/drag-her.gif)

## Row height

By default, the rows in grid view have a short height in order to display at maximum density. If you'd like to see larger attachments and more text per record, you can increase the heights of your rows using the [row height](https://support.airtable.com/hc/en-us/articles/360000359967-Row-height) button.

![row-height.png](https://support.airtable.com/hc/article_attachments/360032848733/row-height.png)

