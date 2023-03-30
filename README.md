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


##**Pick Waves and Release Rules**

https://docs.oracle.com/en/cloud/saas/supply-chain-management/22d/famlo/pick-waves.html#s20032063


## **Shipping Orders**

**Sales order** the orchestration document that represents the demand and supply for items. Sales order lines can be picked, packed, and shipped. Transfer order. This represents the demand and supply for an internal material transfer. Transfer order lines are similar to sales order lines. They can be picked, packed, and shipped.

**Return transfer order** This is a transfer order with the return transaction. The return is performed against the original transfer order. The price and tax for a return transaction order is derived in Oracle Fusion Receiving. Outside processing order. This order is where one or more operations of the work order are outsourced to a supplier who provides specialized manufacturing services. Such work orders are created and released within the Oracle Manufacturing Cloud Solution.

**Return to supply order** A return to supply order is a demand document for shipping items back to a supplier from a fully or partially received purchase order to receive credit for the items. Return to a supplier orders are generated as a result for a return transaction initiated in Oracle Fusion Receiving.

**Dropship order** This is an order where material flows directly from a supplier or contract manufacturer to the customer. The seller relies on the supplier or contract manufacturer to build, store, and ship products to the customer. A dropship purchase order is placed with the supplier, along with instructions to describe how to ship the items, and then the supplier ships directly to the customer.

**Return material authorization** An RMA is a return order used by the customer to return items back to your company. The return is performed against the original sales order. Let's dig a little deeper into the RMA. Here are some values that can be used as the return type for the RMA.

**Cancel the item** Use this value to cancel an item that does not include a shipment. For example, a contract for a wireless phone service typically does not include a shipment. So your customer can't physically return it, but you can cancel it.

**Return for credit** Use this value for an item that your customer can't return or your customer didn't receive the shipment. For example, your customer received the item, but it's severely damaged. 

**Return for credit and return item** Use this value for an item that your customer must return. For example, you customer received an incorrect item from the manufacturer and wants reimbursement. When the manufacturer receives the returned item, the manufacturer issues a credit memo to the customer. 

**Return for repair.** Use this value for your item, your customer request repair.

Transfer order processing is integrated with Oracle Fusion Shipping. You can pick, pack, and ship transfer order lines and shipping. You can also generate shipping documents for a transfer order. Supply Chain Orchestration rules affect transfer order processing when integrating with shipping.

These rules determines if a transfer order is routed directly through Oracle Fusion Shipping or through Oracle Fusion Order Management. Shippable transfer order lines are interfaced to shipping directly from the Transfer Order pages in Oracle Fusion Inventory Management.

### **Oracle Fusion Shipping Transfer Order Processing**
Oracle Fusion Shipping plays a key role in transfer order processing. Below are the parameters that are important components of the transfer order and shipping integration:

- Shipping can generate shipping documentation for transfer order lines. 
- A transfer order line initially maps to one shipment line.
- Ship Confirm updates the shipped quantity on transfer order lines. 
- Shipping can accept a shipment line with internal locations for ship to locations. 
- Shipping validates the updates of shipping-relevant attributes on transfer orders.
- Lines for return transfer orders are treated similar to the ones in the original transfer order, but are identified separately, with an order type of return transfer order. 
- Transfer orders that do not require a physical return or of materials are not interface to shipping. 
- Shipping can generate transfer order shipping costs records to pass to costing.
