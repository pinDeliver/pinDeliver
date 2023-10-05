# Uploading orders from an Excel sheet

A straightforward method for importing orders into pinDeliver is using an Excel sheet. This eliminates the immediate need for integration development, but it's worth noting that this integration task is often a future requirement. Many companies initially begin with Excel import functionality and later advance to phase two, where they establish integrations from their ERP or WMS.

To view a tutorial on Excel upload, watch the video below.
<p float="right">
<a href="https://youtu.be/-K3hSL8nUmM" target="_blank">
<img  alt="Excel Upload" src="/images/excel_order_movieclip_screenshot.png" width="600">
</a>
</p>
The Excel sheet is not restricted to a specific template. Upon uploading the Excel file, you will be prompted to map its columns to corresponding fields within pinDeliver. Subsequently, when you upload another Excel file, pinDeliver will retain your previous field mappings to streamline the process. You only need to confirm that the new file maintains the same structure.

The mandatory fields include: Name, Address, City, and Packages. Packages can be managed in two distinct ways. You can either allocate one column for each package type (description), or you can consolidate all package information into a single cell. If you opt for separate columns for each package type, ensure that these columns are positioned at the far right end of the file.

### Example files ###
Below, you will find two Excel file examples illustrating different approaches to package information representation. The first example illustrates separate columns for the number of boxes and the number of bags. In the second example, these two values are combined within a single cell, with a semicolon serving as the separator.

![Excel example 1](/images/excel_order_example1.png)

![Excel example 2](/images/excel_order_example2.png)

### How to upload Excel ###
Start with **Add order** to access the import pages.

![Excel order 1](/images/excel_order1.png)

Within the import page, you'll first define the *Order name*, *Delivery Group* and *Delivery date*. Then, you can select your Excel file by clicking on **Choose file**. Finally, initiate the upload process by clicking on **Upload Excel file**. If you opt for *Upload to inbox* no order will be immediately generated; this will be handled at a later stage within the inbox.

![Excel order 2](/images/excel_order2.png)

When you import an Excel file for the first time, you will likely encounter numerous red warnings, as you have not yet mapped the Excel columns to their corresponding pinDeliver fields. Mandatory fields that must be mapped include: *Name*, *Address*, *City*, and *Packages*.

![Excel order 3](/images/excel_order3.png)

In the example below, the following fields have been mapped in sequential order:
* Tracking number
* Customer's name
* Address
* Zip
* City
* Mobile phone
* Customer info 1
* Time window start
* Time window end
* Weight units
* Volume units
* Packages start (use *Packages* instead if two values are merged in one column)
* (Not selected) - (since *Packages start* is selected)

Once you have mapped the desired columns (please note that mapping all columns is not mandatory), you can proceed by clicking on **Create order**. If these orders are intended for a *Click & Collect* order, you must first select *Make the order a collection order*. Failure to do so will require you to restart the import process.

![Excel order 4](/images/excel_order4.png)

If all orders feature accurate addresses that can be matched with acceptable latitude and longitude coordinates, you will be directed to the optimization page. Here, you can choose which vehicles you would like to use, as demonstrated below. If you prefer not to perform route optimization at this moment, simply click **Cancel** to proceed with importing your customer orders without routing optimization.

![Excel order 5](/images/excel_order5.png)

To read more about route optimization, navigate to [Route planning](route_optimization_transport_planning.md).
