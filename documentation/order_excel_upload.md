# How to upload orders from an Excel sheet

A simple way to import orders to pinDeliver is through an Excel sheet. Then you don't need to develop an integration but on the other hand this task is always needed. Some companies start with the Excel import functionality and then develop an integration from their ERP or WMS as phase 2.

Click the image below to see a clip about Excel upload:
<p float="right">
<a href="https://youtu.be/-K3hSL8nUmM" target="_blank">
<img  alt="Excel Upload" src="/images/excel_order_movieclip_screenshot.png" width="600">
</a>
</p>
The Excel sheet doesn't need to match a specific template. When you upload the Excel file you will need to map columns to fields in pinDeliver. The next time you upload an Excel file again you will see that pinDeliver remember your last field mapping so you only have to confirm that this file has the same structure. Mandatory fields are: Name, Address, Zip code, City and Packages. Packages can be handled in  two different ways. You can have one column for each package type (description) or you can have one column with all information in the same cell. If you have one column for each package type these columns must be at the end of the filed (to the right).

### Example files ###
Below you see example of two different Excel files. The first example shows package information in how packages are represented. In the first example you see two different columns, one column for number of *boxes* and another column for number of *bags*. In the second example those two values are merged in one column and separated with semicolon. The process below will show the first example.

![Excel example 1](/images/excel_order_example1.png)

![Excel example 2](/images/excel_order_example2.png)

### How to upload Excel ###
Start by clicking **Add order** to open the import pages.

![Excel order 1](/images/excel_order1.png)

In the import page you specify *Order name*, *Delivery Group* and *Delivery date* before you select your Excel file by clicking **Choose file**. After that you click **Upload Excel file**. If you choose *Upload to inbox* no order will be created. That will be done from the inbox later.

![Excel order 2](/images/excel_order2.png)

If it is the first time you import an Excel file you will see a lot of red warnings since you have not yet mapped the Excel columns to pinDeliver fields. Mandatory fields are: Name, Address, Zip code, City and Packages.

![Excel order 3](/images/excel_order3.png)

In this example I have chosen to map the following fields (in order):
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
* Packages start (if the field would be as in example 2 you use *Packages* instead)
* (Not selected) - since we use *Packages start*

When you have mapped all columns you want (you do not need to map all columns) you click **Create order**. If these orders are supposed to be collected by the customer you need to select *Make the order a collection order* first, otherwise you will need to do the import all over.

![Excel order 4](/images/excel_order4.png)

If all orders have correct addresses that can be looked up with acceptable latitude and longitude you will be directed to the optimization page where you can select with vehicles you want to use. See below.
If you don't want to route optimize right now you can just click **Cancel** to just import your customer orders.

![Excel order 5](/images/excel_order5.png)

To learn about route optimization just go to [Route planning](route_optimization_transport_planning.md).
