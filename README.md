# 🍉 Tesco UK & Ireland Grocery Scraper

![Tesco Grocery Products Scraper Cover Image](https://i.imgur.com/7TZiiH2.png)
| Try our other scrapers ► | [Glassdoor Scraper](https://apify.com/radeance/glassdoor-jobs-scraper) | [Wellfound Premium Job Scraper](https://apify.com/radeance/wellfound-job-listings-scraper)| [Similarweb Scraper](https://apify.com/radeance/similarweb-scraper)
|----------------------------|-----------------------------|-----------------------------|-----------------------------|

<br>

This blazing fast & powerful scraper is designed to effortlessly scrape grocery product data from **Tesco UK** & **Tesco Ireland**, the UK’s largest supermarket. Perfect for shoppers, market researchers, and retail businesses, it extracts **detailed product insights**, including **UPCs / GTINs** , **prices**, **promotions**, **nutrition**, **allergens**, **manufacturer details**, and **competitor matching price data**

It supports **category listing** pages and **product** URLs in one go, making it easy to scrape any grocery product with automatic pagination at scale.
<br><br>Get the data you need in record time and stay ahead of the market! 🥂

### [Try it out today for free on Apify! ](https://apify.com/radeance/tesco-scraper)

## Key features

-   **🔍 Product Data**
    -   Scrapes any grocery product from Tesco UK
    -   Extracts detailed product data in seconds
    -   Provides key details such as - **Product title**, - **UPC/GTIN**, - **Price**, - **Offer / Promotion prices**, - **Unit prices**, - **Description**, - **Main / Sub / Product Categories**, - **Nutritional information**, - **Allergens**, - **Manufacturer information**, - **Price matching data**
        <br>
-   **⚡ Fast and Efficient:**
    -   Extremely fast, scraping 1000 data entries in a minute
        <br>
-   **📝 Product Category Listings Support**

    -   Scrape grocery product categories by providing one or multiple category urls
    -   Automatic pagination until `max_items` scraping limit is reached
        <br>

-   **📊 Flexible Data Output**
    -   Outputs data in various formats including CSV, XLSX, JSON, JSONL, XML, and RSS

### 📌 UI Input

#### Supported URL Formats

| URL format                                                  | Supported |
| ----------------------------------------------------------- | --------- |
| `https://www.tesco.com/groceries/en-GB/products/272202380`  | ✅        |
| `https://www.tesco.com/groceries/en-GB/shop/fresh-food/all` | ✅        |

#### Supported Tesco Regions

| Region                           | Supported |
| -------------------------------- | --------- |
| Tesco United Kingdom (tesco.com) | ✅        |
| Tesco Ireland (tesco.ie)         | ✅        |

![Tesco Scraper Input](https://i.imgur.com/rI5hoyj.png)

-   `category`: (Required) (String) (Default: fresh-food)
    Enter your desired listings or product urls in bulk or a single product url
    <br>
-   `region`: (Required) (String) (Default: UK)
    Enter your desired tesco region you want to scrape from.
    <br>
-   `urls`: (Optional) (String Array)
    Enter your desired listings or product urls in bulk or a single product url
    <br>
-   `include_product_details`: (Optional) (Boolean) (Default: True)
    Include scraping product page details for listing urls
    <br>
-   `max_items`: (Optional) (Number) (Default: 100)
    Enter the number of items you want to be retrieved ⚠️ Free Users will be limited to 100
    <br>
-   `max_pages`: (Optional) (Number) (Default: 1)
    Enter the number of pages you want the scraper to go trough ⚠️ Free Users will be limited to 5
-   `page_offset`: (Optional) (Number) (Default: 1)
    Enter page number you want the scraper to start from ⚠️ Paid-Only Feature. Free Users will be limited to 1

    #### ✏️ OR via JSON Input

    Sample JSON input if you use the apify api via CURL, Python, JS etc.
    ![Tescp Scraper JSON Input](https://i.imgur.com/qegGSTb.png)

### 📎 Detailed Output Information

-   **Product Details:**

    -   **Product ID:** Unique identifier for the product.
    -   **Base Product ID:** Identifier for the base product group.
    -   **SKU:** Stock Keeping Unit number.
    -   **GTIN:** Global Trade Item Number.
    -   **Brand Name:** The brand associated with the product.
    -   **Name:** Full name and description of the product.
    -   **Description:** Detailed description of the product.
    -   **Price:** The current price of the product.
    -   **Currency:** Currency in which the price is listed.
    -   **In Stock:** Availability status of the product.
    -   **Promotion:** Details of any ongoing promotions, including promotion ID, description, discount price, discount percentage, unit price information, and terms.

-   **Unit Information:**

    -   **Unit:** Measurement unit (e.g., ML, G).
    -   **Unit Price:** Price per measurement unit.
    -   **Unit Quantity:** Total quantity in the specified unit.

-   **Media:**

    -   **Image URL:** Direct link to the product's image.
    -   **URL:** Direct link to the product's page on the grocery website.

-   **Purchase Restrictions:**

    -   **Buy Limit:** Maximum quantity allowed per purchase.
    -   **Buy Limit Message:** Message displayed regarding purchase limits.

-   **Product Attributes:**

    -   **Is New:** Indicates if the product is new.
    -   **Sale Type:** Type of sale (e.g., SingleProduct).
    -   **Main Category:** Primary category under which the product is listed.
    -   **Sub Category:** Sub-category for more specific classification.
    -   **Product Category:** Detailed product category.
    -   **Product Type:** Specific type of product.

-   **Ingredients and Allergens:**

    -   **Ingredients:** List of ingredients used in the product.
    -   **Allergens:** Information about potential allergens present in the product.

-   **Usage and Storage:**

    -   **Storage Instructions:** Guidelines for storing the product.
    -   **Usage Instructions:** Detailed instructions for product usage.

-   **Nutrition Information:**

    -   **Nutrition:** Detailed nutritional information including typical values and percentages per serving.

-   **Manufacturer Details:**

    -   **Manufacturer:** Information about the manufacturer, including name, address, email, phone, and website.

-   **Additional Information:**

    -   **Additional Information:** Any other relevant information about the product.
    -   **Marketing Text:** Promotional and marketing descriptions for the product.

-   **Export Formats:** Data can be exported in various formats including CSV, XLSX, JSON, JSONL, XML, and RSS for easy integration and analysis.

#### Output Data Sample

**Overview Table**
![Tesco Scraper Output](https://i.imgur.com/0fVDSMW.png)
**JSON**

```json
{
    "product_id": "250808808",
    "base_product_id": "55238977",
    "sku": "250808808",
    "gtin": "05011037611195",
    "brand_name": "DAIRYGOLD",
    "name": "Dairygold Original 454G",
    "description": "Blended spread 63%.",
    "price": 3.59,
    "currency": "GBP",
    "isLowEverydayPricing": false,
    "isLowPricePromise": false,
    "in_stock": true,
    "promotion": {
        "promotion_id": "91947589",
        "description": "€3.00 Clubcard Price",
        "discount_price": null,
        "discount_percentage": null,
        "unit_price_info": "€6.61/kg",
        "unit_price": null,
        "unit_quantity": null,
        "valid_from": "2025-05-13T23:00:00Z",
        "valid_to": "2025-06-10T23:00:00Z",
        "terms": "CLUBCARD_PRICING"
    },
    "price_matches_competitor": true,
    "competitors": ["Aldi"],
    "unit": "G",
    "unit_price": 7.91,
    "unit_quantity": "454",
    "servings": "This pack contains 45 servings",
    "netContents": "454g ℮",
    "drainedWeight": null,
    "dosage": null,
    "prepartionAndUsage": null,
    "preparationGuidelines": null,
    "cookingInstructions": [],
    "freezingInstructions": null,
    "directions": null,
    "features": [
        "Traditionally Made Using Natural Ingredients",
        "Perfectly churned, deliciously creamy, Dairygold taste",
        "Contains no hydrogenated oils",
        "Guaranteed Irish",
        "Suitable for vegetarians"
    ],
    "healthClaims": null,
    "boxContents": null,
    "nutritionalClaims": null,
    "otherInformation": null,
    "additives": null,
    "recyclingInfo": null,
    "safetyWarning": null,
    "warnings": null,
    "originInformation": null,
    "image_url": "https://digitalcontent.api.tesco.com/v2/media/ghs/9f5f1197-70f0-48b8-8dfd-20e0462655c6/942bbe24-1e12-488a-abf1-e9bee337dfdf_1597895882.jpeg",
    "url": "https://www.tesco.ie/groceries/en-IE/products/250808808",
    "buy_limit": 99,
    "buy_limit_message": "Max allowed is 99.",
    "is_new": false,
    "sale_type": "SingleProduct",
    "main_category": "Fresh Food",
    "sub_category": "Milk, Butter & Eggs",
    "product_category": "Butter, Spreads & Margarine",
    "product_type": "Butter",
    "product_attributes": ["Vegetarian"],
    "ingredients": "Cream, Palm Oil, Rapeseed Oil, Salt, Colour (Carotenes)",
    "allergens": "For allergens see ingredients in bold",
    "storage_instructions": ["Keep refrigeratedBest Before: See Lid"],
    "usage_instructions": null,
    "nutrition": {
        "Measure": "100g contains",
        "Energy kJ": "2392kJ",
        "Energy kcal": "582kcal",
        "Fat": "63g",
        "(of which saturates)": "21g",
        "Carbohydrate": "1.0g",
        "(of which sugars)": "<0.5g",
        "Protein": "0.5g",
        "Salt": "1.34g",
        "* RI - Reference Intake of an average adult (8400kJ/2000kcal)": "-"
    },
    "nutrition_per_serving": {
        "Measure": "10g contains",
        "Energy kJ": "239kJ",
        "Energy kcal": "58kcal",
        "Fat": "6.3g",
        "(of which saturates)": "2.1g",
        "Carbohydrate": "<0.5g",
        "(of which sugars)": "<0.5g",
        "Protein": "<0.5g",
        "Salt": "0.13g",
        "* RI - Reference Intake of an average adult (8400kJ/2000kcal)": "-"
    },
    "manufacturer": {
        "name": "Kerry EMEA,",
        "adress": "Naas,Co. Kildare,W91 W923,Ireland.",
        "email": null,
        "phone": null,
        "website": null
    },
    "additional_information": null,
    "marketing_text": null
}
```

## ✨ You can try it out for free

1. Create a free Apify Account
2. Go to the Inputs Tab on this Scraper
3. Enter Product Detail Page Urls or Category Listing Urls
4. Press Start
5. Happy scraping ! 🚀

### Use Cases | What it can be used for

-   **Bulk Product Data Collection**: Efficiently scrape large volumes of grocery product data
-   **Price Comparison**: Extract and compare prices across different products and brands to find the best deals.
-   **Market Analysis**: Analyze product data to understand market trends, popular brands, and product categories.
-   **Promotion Tracking**: Identify and track promotional offers and discounts on various products.
-   **Product Detail Extraction**: Collect comprehensive details such as product ID, SKU, GTIN, brand name, description, price, and unit quantity.
-   **Stock Availability Monitoring**: Check the in-stock status of products to maintain up-to-date availability information.
-   **Nutritional Information**: Extract and store nutritional data for health and diet analysis.
-   **Allergen Warnings**: Gather allergen information to ensure product safety for consumers with specific dietary requirements.
-   **Manufacturer Details**: Collect manufacturer information including name, address, email, and website for reference and contact purposes.
-   **Categorization**: Classify products into main categories, sub-categories, and product types for better organization and searchability.

### ⚙️ While the scraper is running

During the run, the actor will output log messages letting you know what is going on at any point. Each message always contains specific information about the process including which url / page the actor is working on.

If you provide invalid inputs to the actor, it will immediately stop with a failure state and output log messages explaining what is wrong. If you are unsure what went wrong feel free to open up an issue in the issue tab.

## 🔗 Legality of web scraping and scraping of grocery store products

The **Tesco UK Scraper** is designed to ethically extract **only publicly available product data and manufacturer information**, and it **does not** scrape private user data such as personal email addresses or personal identifiers.

Our scrapers are ethical and do not extract any private user data, such as email addresses, gender, or location. They only extract what the user has chosen to share publicly. We therefore believe that our scrapers, when used for ethical purposes by Apify users, are safe. However, you should be aware that your results could contain personal data. Personal data is protected by the GDPR in the European Union and by other regulations around the world. You should not scrape personal data unless you have a legitimate reason to do so. If you're unsure whether your reason is legitimate, consult your lawyers. You can also read our [blog post](https://blog.apify.com/is-web-scraping-legal/) on the legality of web scraping

## 💬 Feedback and Support

**Your satisfaction** is **important** to us! Therefore we are constantly striving to enhance the performance of our Actors.

If you have any technical feedback or encounter any bugs with the Tesco UK Scraper, please create an issue in the Actor’s Issues tab on the Apify Console.

You can also contact us directly for custom integrations or project use cases at business@radeance.com.

Thank you and happy scraping!


### [Try it out today for free on Apify! ](https://apify.com/radeance/tesco-scraper)