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

# Business Objectives

- What times do we tend to be busiest?
- How many pizzas are we making during peak periods?
- What is the order performance of our various pizza sizes?
- What is our monthly revenue and order performance?
- What are our best and worst-selling pizzas?
- Which of our Pizza Category is the most in demand?
- What's our average Revenue?

# Analysis

Analysis was done on SQL and visualized on Tableau. I used SQL to extract, transform and convert the Pizza data. I uploaded the dataset first on SQL Server where I did all the analysis before visualizing it on Tableau.

This is the full [Analysis](https://github.com/mohammadeimon/SQLProjects/blob/main/PizzaRestaurant.sql)

# Findings

Year - 2015

Number_of_pizza_types - 32	

Total_Orders - 48,620	

Total_Quantity_Sold	- 49,574

Total_revenue - $817,860.05	

Average_revenue - $16.82


- The period between 12pm and 1pm (lunchtime) is the most hectic time of the day. During 12pm, the restaurant received a total of 6,543 orders and made 6,776 pizzas, resulting in revenue of $111,877.9. At 1pm, the restaurant received 6,203 orders and made 6,413 pizzas, generating $106,065.7 in revenue.

![1](https://user-images.githubusercontent.com/123791304/235460344-ae56d76f-4852-4c0c-84df-5823d9172a40.PNG)


- The Large Size pizza is the most popular among customers, with a total of 18,526 orders placed for it. The restaurant sold 18,956 quantities of this pizza size, generating revenue of $375,318.7. In contrast, the least popular pizza size is XXL, with only 28 orders and 28 quantities sold, resulting in revenue of $1,006.6.

![2](https://user-images.githubusercontent.com/123791304/235463614-00cecfb6-900f-472d-90dd-4f5027a68bf8.jpg)

- The month of July is the most successful, with a total of 4,301 orders placed and 4,392 pizzas sold, generating revenue of $72,557.9. On the other hand, the month of October is the least successful, with only 3,797 orders placed and 3,883 pizzas sold, resulting in revenue of $64,027.6.

![image](https://user-images.githubusercontent.com/123791304/235464579-86ee0cf0-c406-496c-b106-41fa2929449c.png)

- The Classic Deluxe Pizza is our most popular pizza overall. It has been ordered 2,416 times, with a total of 2,453 pizzas sold, resulting in revenue of $38,180.5. In contrast, the worst-selling pizza is The Brie Carre Pizza, with only 480 orders and 490 pizzas sold, generating revenue of $11,588.5.

![4](https://user-images.githubusercontent.com/123791304/235464983-bfbb7f15-3d48-4988-8979-f53e20760be6.jpg)

- The busiest days of the week are Friday and Saturday, which mark the beginning of the weekend. On Fridays, the restaurant received a total of 8,106 orders, made 8,242 pizzas, and generated revenue of $136,073.9. Saturdays are also busy, with a total of 7,355 orders received, 7,493 pizzas made, and revenue generated totaling $123,182.4.

![5](https://user-images.githubusercontent.com/123791304/235464991-ad47a393-ee5c-4004-95d0-afb258c102b2.jpg)

- The Classic pizza category is the most popular, with 14,579 orders placed for it. The restaurant sold a total of 14,888 pizzas from this category, resulting in revenue of $220,053.1.

![6](https://user-images.githubusercontent.com/123791304/235465508-ec0c5d88-c4e5-4c50-a274-5e1b380af24b.jpg)


# Visualization

[Tableau](https://public.tableau.com/app/profile/mohammad.eimon/viz/PizzaSaleDashboard/Dashboard1?publish=yes)

![Pizza Dashboard image](https://user-images.githubusercontent.com/123791304/235674923-996ed9ff-8cd1-4463-b848-11a72f9f7133.png)



# Conclusion
Pizza orders and revenue typically increase steadily from Sunday and peak on Friday before starting to decline, indicating that many people prefer to eat pizza towards and during the weekend. On Fridays, most people prefer to have the Pepperoni pizza for lunch. Therefore, it is advisable to make tables and chairs available to accommodate the expected weekend influx of customers, and exploring delivery services is also a good option. Also, the pizza menu needs a little trim removing the least popular pizza and the company would greatly benefit from seasonal and weekday promotions to keep customer engagement.  

To meet the demand for Pepperoni pizza on Fridays, it's essential to ensure that its ingredients are readily available and in large quantities before the day. Since more orders are received on Fridays, it could be beneficial to introduce a discount policy on the last Friday of every month. This policy could give customers an extra pizza when they buy three or more, encouraging them to buy more and increasing revenue.
