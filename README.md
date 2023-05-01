# Pizza-Sales-Analysis

# Introduction

[Kaggle](https://www.kaggle.com/datasets/shilongzhuang/pizza-sales)

Things are going OK here at Plato's, but there's room for improvement. They've been collecting transactional data for the past year, but really haven't been able to put it to good use. Hoping we can analyze the data and put together a report to help us find opportunities to drive more sales and work more efficiently.


This pizza sales dataset make up 12 relevant features:

  order_id: Unique identifier for each order placed by a table

  order_details_id: Unique identifier for each pizza placed within each order (pizzas of the same type and size are kept in the same row, and the quantity increases)

  pizza_id: Unique key identifier that ties the pizza ordered to its details, like size and price

  quantity: Quantity ordered for each pizza of the same type and size

  order_date: Date the order was placed (entered into the system prior to cooking & serving)

  order_time: Time the order was placed (entered into the system prior to cooking & serving)

  unit_price: Price of the pizza in USD

  total_price: unit_price * quantity

  pizza_size: Size of the pizza (Small, Medium, Large, X Large, or XX Large)

  pizza_type: Unique key identifier that ties the pizza ordered to its details, like size and price

  pizza_ingredients: ingredients used in the pizza as shown in the menu (they all include Mozzarella Cheese, even if not specified; and they all include Tomato Sauce,   unless another sauce is specified)

  pizza_name: Name of the pizza as shown in the menu

# Business Tasks

- What days and times do we tend to be busiest?
- How many pizzas are we making during peak periods?
- What are our best and worst-selling pizzas?
- What's our average Revenue?
- What is our monthly order performance?
- What is the order performance of our various pizza sizes?
- Which of our Pizza Category is the most in demand?
- What is our monthly revenue performance?
- Provide a quick visualization for the Month on Month breakdown of our Revenue vs Orders

# Analysis

Analysis was done on SQL and visualized on Tableau. I used SQL to extract, transform and convert the Pizza data. I uploaded the dataset first on SQL Server where I did all the analysis before visualizing it on Tableau.

This is the full [Analysis]((https://github.com/mohammadeimon/SQLProjects/blob/main/PizzaRestaurant.sql))

# Findings

Year considered - 2015

Total_Orders - 48,620	

Number_of_pizza_types - 32	

Total_Quantity_Sold	- 49,574

Total_revenue - $817,860.05	

Average_revenue - $16.82


- The busiest time of the day is between 12pm and 1pm which is Lunch period. For 12pm, a total of 6,543 orders was received, 6,776 quantites of Pizzas were made and revenue generated was $111,877.9 while for 1pm, a total of 6,203 orders was received, 6,413 quantities of Pizza made and revenue generated was $106,065.7.

![1](https://user-images.githubusercontent.com/123791304/235460344-ae56d76f-4852-4c0c-84df-5823d9172a40.PNG)


- The highest sold pizza size is the Large Size with a total of 18,526 orders placed for it,	18,956 quantites sold and revenue generation of $375,318.7, the least sold pizza size is the XXL with just 28 orders, 28 quantities sold and $1,006.6 revenue generated.


![2](https://user-images.githubusercontent.com/123791304/235463614-00cecfb6-900f-472d-90dd-4f5027a68bf8.jpg)

- July is the top performing month with a total of 4,301 orders, 4,392 pizzas sold and revenue generation of $72,557.9. The least performing month is October with 3,797 orders, 3,883 quantities of pizza sold and revenue generation of $64,027.6.

![image](https://user-images.githubusercontent.com/123791304/235464579-86ee0cf0-c406-496c-b106-41fa2929449c.png)

- Our overall best selling pizza is The Classic Deluxe Pizza. It was ordered 2,416 times, a total of 2,453 quanties was sold and it generated revenue of $38,180.5. The worst selling pizza is The Brie Carre Pizza	with a total of just 480 orders, 490 quantities made and revenue of	$11,588.5.

![4](https://user-images.githubusercontent.com/123791304/235464983-bfbb7f15-3d48-4988-8979-f53e20760be6.jpg)

- The busiest days are Fridays and Saturdays (Beginning of the weekend). With Fridays having a total of 8,106 orders, 8,242 quantities of pizzas made, and revenue generation of $136,073.9. While on Saturdays, orders received was 7,355, with a total of 7,493 pizzas made and revenue generation of $123,182.4.

![5](https://user-images.githubusercontent.com/123791304/235464991-ad47a393-ee5c-4004-95d0-afb258c102b2.jpg)

- The pizza category which is most in demand is the Classic	with 14,579 orders placed for it, 14,888 quantities sold and	$22,0053.1 revenue generated.

![6](https://user-images.githubusercontent.com/123791304/235465508-ec0c5d88-c4e5-4c50-a274-5e1b380af24b.jpg)


# Visualization

[Tableau](https://public.tableau.com/app/profile/mohammad.eimon/viz/PizzaSaleDashboard/Dashboard1?publish=yes)

![Pizza Dashboard image](https://user-images.githubusercontent.com/123791304/235468349-768e8bd7-5b3c-4481-9028-7514c6e78977.png)



# Conclusion
Pizza orders and revenue maintains an upward trajectory from the beginning of the week Sunday and peaks on Friday before it starts dropping, this means most people prefer to eat pizza towards and during the weekend. Most people prefer to have the Pepperoni pizza for lunch on Fridays. It is advisable to make available tables and chairs to be able to accomodate the influx of the weekend, we can also explore the option of delivery services. The Ingrdients for  Pepperoni pizza should be made readily available and in large quantities on or before Fridays. Since more orders are received on Fridays, a discount policy can be introduced every last Friday of the month where a customer gets 1 extra pizza when they buy 3 and above, this will encourage them to buy more. 
