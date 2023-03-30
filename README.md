# Oracle Products 


## Oracle Order Management

### Order to Cash

Receive Order --> Fill Order --> Ship Order --> Create Invoice --> Receive Payment --> Record Payment



![Image of O2C](https://github.com/IamVigneshC/Oracle/blob/main/Resources/OrderToCash.png)


## Shipment

The type of shipping documents that you will have the option to use include an 

**advance shipping notice**-- this is transmitted via EDI from a supplier to let the receiving organization know that a shipment is coming; 

**a packing slip**-- this is a listing of the items packed within a particular carton. The packing slips can be especially useful for shipments that are packed into multiple cartons; 

**the bill of lading**-- the bill of lading lists all items in a shipment destined for a particular ship-to location; and 

**a commercial invoice**-- this is a customs document that lists all confirmed shipping items in a delivery, shipments date, commercial invoice ID, shipper and exporters, ship-to address, exporter ID numbers, freight carriers, country of origin, and all the information it would need to accompany.


### **A drop ship**

**A drop ship** is an order fulfillment strategy where the seller does not keep products in inventory, but instead, they rely on suppliers or contract manufacturers to build, store, and ship orders directly to the customers.

You may choose to fulfill drop shipment orders due to a lack of warehouse availability or if an item is customized at a supplier site. Drop shipping directly to the customer from the supplier saves time and money. When a customer places an order for a shipped product, the seller issues a purchase order for the item and provides instructions for shipping directly to the customer.

Then, the supplier ships the product directly to the customer. The shipping manager can still print the packing slips, bill of lading, and commercial invoice for drop shipments, and shipping instructions can be sent manually to the supplier either with the shipping paperwork or by email. The supplier, in turn, sends the paperwork to the customer.

**How can I send an ASN for a drop ship order?**

A customer advance shipping notice, otherwise known as an ASN, is created when the warehouse manager or supplier creates an ASN for a drop ship order. You can send this ASN to the customer using Integrated Cloud Service Integration or Business-to-business Messaging using Oracle Collaboration Messaging Framework which is providing the customer has enabled it.

ICS is an end-to-end integration orchestration platform that simplifies how to use and apply product integrations offered within the Cloud. Oracle Fusion Collaboration Messaging Framework provides the ability to manage business-to-business communication with a large number of suppliers.

**What's the difference between a purchase order return and a drop ship purchase order return?**

For a regular purchase order return, you can return goods to either receiving or the supplier. For a drop ship purchase order return, you can only return goods to the supplier. You cannot return goods to receiving.

