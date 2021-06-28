# Roberto il Pizzaiolo 🍕

Our fearless CEO Roberto has been passionately running 3 pizzeria's in Northern California using only the freshest of ingredients. As a crowd favorite, the classic Margherita pizza (where ingredients are critical to the quality) is the only pizza on the menu.

## Problemo

So what's the deal?

Every ingredient vendor has a different schedule, price, communication channel, and technical sophistication when it comes to ordering. Roberto is managing his entire ingredient ordering process in Excel 🤯. Last week his West Oakland spot was low-on-dough and had to turn down customer orders. Not ideal.

To make matters even more fun, Roberto wants to expand and **open 5 more pizzerias this year**—his ordering problem is going to increase exponentially!


### Ingredient Delivery
| Ingredient  | Vendor | Update / Order Source | Update Frequency |
| ------------- | ------------- | ------ | ------ | 
| Yeast  | Prop Labs Kolsch Beer Yeast | REST API | Manual Daily Updates |
| Olive Oil | Crudo Ogliarolo | Phone Call (Twilio-like API) | International Freight Delivery Mass Updates |
| Tomatoes | San Marzano Whole Tomatoes | Webhook Push | Live Updates |
| Mozzarella | Sonoma Farms | Text (Twilio-like API) | Sporadic Updates |
| Basil | Oakland Farmer's Market | Weekly Email | Seasonal Updates | 


## Design take-home test
Design a one-page screen in Figma showing Roberto's daily dashboard for him to understand a few important updates. Please share messy, design process Figma files so we get a sense of how you think. The sloppier the better.

1. In some type of schedule view, what's the next delivery he should be expecting? And what's the past deliveries he's received?
2. What's the latest for each individual vendor? Does he need to follow up with anyone to get updated information?
3. What's the current inventory? Can we use the existing excel workflow and bring it online to inform our ingredient forecasting?
4. Can you render the data in a chart or visual format?

## Full stack take-home test
Build a filterable, sortable table view in React using mock data that would call to a simple Ruby API (Ruby API can be a simple Sinatra file, pseudo code, or return mock data).

Add one little special feature that you personally think is important in developing features (examples: animations, security, graphql, testing, service object, etc).

Our app is written in Next.js but feel free to use Create React App or Code Sandbox.

Once you're finished please invite me to the repo and send a quick email. Github username: `moeamaya`

## Backend Ruby take-home test
Design and build an `InventoryJob` (and include any other Ruby classes that you need) to fetch data from the different vendors, sources, and update frequencies. The job will run every hour to update our database (you don't need to handle the database, only create the job and whatever you need to fetch the data).

We're big fans of Sandi Metz and her [SOLID Object-Oriented design](https://sandimetz.com/blog/2009/03/21/solid-design-principles) but feel free to implement in the style you're most comfortable with.

Please write a test to handle your primary methods in each class.

For the external API calls, you can assume the job is already authenticated, and you're just calling a get method to return data back in json (`TextAPI.get_texts`, etc).

Once you're finished please invite me to the repo and send a quick email. Github username: `moeamaya`
