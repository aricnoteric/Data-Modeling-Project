<h2>Data Modeling Project</h2>
In this project, the aim is to predict the total delivery time for DoorDash orders. When a consumer places an order on DoorDash, they are shown the expected time of delivery - it is very important that the service gets this time right as it has a big impact on consumer experience and can affect if they continue using the service or not. The time is calculated from when the consumer submits the order to when the order is delivered to the conusmer.

The dataset we have are deliveries made in 2015, and we will be creating a machine learning model to predict the total delivery time for new orders.

<h2>Data Description</h2>
The dataset provided is historical_data.csv. Each row in the file corresponds to one unique delivery, and each column corresponds to a feature explained below:

<ul>
    <li>market_id: A city/region in which DoorDash operates, e.g., Los Angeles, given in the data as an id
    <li>created_at: Timestamp in UTC when the order was submitted by the consumer to DoorDash. (Note this timestamp is in UTC, but in case you need it, the actual timezone of the region was US/Pacific)
    <li>actual_delivery_time: Timestamp in UTC when the order was delivered to the consumer
    <li>store_id: an id representing the restaurant the order was submitted for
    <li>store_primary_category: cuisine category of the restaurant, e.g., italian, asian
    <li>order_protocol: a store can receive orders from DoorDash through many modes. This field represents an id denoting the protocol
    <li>total_items: total number of items in the order
    <li>subtotal: total value of the order submitted (in cents)
    <li>num_distinct_items: number of distinct items included in the order
    <li>min_item_price: price of the item with the least cost in the order (in cents)
    <li>max_item_price: price of the item with the highest cost in the order (in cents)
    <li>total_onshift_dashers: Number of available dashers who are within 10 miles of the store at the time of order creation
    <li>total_busy_dashers: Subset of above total_onshift_dashers who are currently working on an order
    <li>total_outstanding_orders: Number of orders within 10 miles of this order that are currently being processed.
    <li>estimated_order_place_duration: Estimated time for the restaurant to receive the order from DoorDash (in seconds)
    <li>estimated_store_to_consumer_driving_duration: Estimated travel time between store and consumer (in seconds)
    <li>The target variable for our prediction task is the actual_total_delivery_time, which is the time between created_at and actual_delivery_time.
</ul>
        