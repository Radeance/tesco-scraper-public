
# 🛒 Tesco UK Discover Grocery Scraper

## ⌲ Premium Grocery Scraper

[Try it out today for free on Apify! ](https://apify.com/radeance/tesco-scraper)

![Tesco Grocery Products](https://i.imgur.com/0bWNJ56.png)

### What does Tesco Discover Grocery Scraper do?

Tesco Discover Grocery Scraper is a comprehensive tool that extracts grocery product-related data from [Tesco UK](https://www.tesco.com), UKs largest supermarket. Using the unique URLs of product urls, the scraper runs through, capturing key product information about prices, nutrition, offers, and corresponding manufacturing details.

This premium blazing fast and powerful tool is designed to effortlessly scrape grocery products from Tesco UK. It simply is the **best grocery product scraper on the market**.
Perfect for individuals, market researchers and analysts, as well as retail businesses.


## Key features


- **🔍 Product Data**
  - Scrapes any grocery product from Tesco UK
  - Extracts detailed product data in seconds
  - Provides key details such as 
    - **Product title**,
    - **UPC/GTIN**,
    - **Price**,
    - **Offer / Promotion prices**,
    - **Unit prices**,
    - **Description**,
    - **Main / Sub / Product Categories**,
    - **Nutritional information**,
    - **Allergens**,
    - **Manufacturer information**,
    - **Price matching data**
<br>
- **⚡ Fast and Efficient:**
  - Extremely fast, scraping 1000 data entries in a minute
<br>
- **📝 Product Listings Support**
  - Listings support including pagination coming very soon
<br>

- **📊 Flexible Data Output**
  - Outputs data in various formats including CSV, XLSX, JSON, JSONL, XML, and RSS

### Use Cases | What it can be used for

- **Bulk Product Data Collection**: Efficiently scrape large volumes of grocery product data
- **Price Comparison**: Extract and compare prices across different products and brands to find the best deals.
- **Market Analysis**: Analyze product data to understand market trends, popular brands, and product categories.
- **Promotion Tracking**: Identify and track promotional offers and discounts on various products.
- **Product Detail Extraction**: Collect comprehensive details such as product ID, SKU, GTIN, brand name, description, price, and unit quantity.
- **Stock Availability Monitoring**: Check the in-stock status of products to maintain up-to-date availability information.
- **Nutritional Information**: Extract and store nutritional data for health and diet analysis.
- **Allergen Warnings**: Gather allergen information to ensure product safety for consumers with specific dietary requirements.
- **Manufacturer Details**: Collect manufacturer information including name, address, email, and website for reference and contact purposes.
- **Categorization**: Classify products into main categories, sub-categories, and product types for better organization and searchability.


### 📎 Detailed Output Information

- **Product Details:**
  - **Product ID:** Unique identifier for the product.
  - **Base Product ID:** Identifier for the base product group.
  - **SKU:** Stock Keeping Unit number.
  - **GTIN:** Global Trade Item Number.
  - **Brand Name:** The brand associated with the product.
  - **Name:** Full name and description of the product.
  - **Description:** Detailed description of the product.
  - **Price:** The current price of the product.
  - **Currency:** Currency in which the price is listed.
  - **In Stock:** Availability status of the product.
  - **Promotion:** Details of any ongoing promotions, including promotion ID, description, discount price, discount percentage, unit price information, and terms.

- **Unit Information:**
  - **Unit:** Measurement unit (e.g., ML, G).
  - **Unit Price:** Price per measurement unit.
  - **Unit Quantity:** Total quantity in the specified unit.

- **Media:**
  - **Image URL:** Direct link to the product's image.
  - **URL:** Direct link to the product's page on the grocery website.

- **Purchase Restrictions:**
  - **Buy Limit:** Maximum quantity allowed per purchase.
  - **Buy Limit Message:** Message displayed regarding purchase limits.

- **Product Attributes:**
  - **Is New:** Indicates if the product is new.
  - **Sale Type:** Type of sale (e.g., SingleProduct).
  - **Main Category:** Primary category under which the product is listed.
  - **Sub Category:** Sub-category for more specific classification.
  - **Product Category:** Detailed product category.
  - **Product Type:** Specific type of product.

- **Ingredients and Allergens:**
  - **Ingredients:** List of ingredients used in the product.
  - **Allergens:** Information about potential allergens present in the product.

- **Usage and Storage:**
  - **Storage Instructions:** Guidelines for storing the product.
  - **Usage Instructions:** Detailed instructions for product usage.

- **Nutrition Information:**
  - **Nutrition:** Detailed nutritional information including typical values and percentages per serving.

- **Manufacturer Details:**
  - **Manufacturer:** Information about the manufacturer, including name, address, email, phone, and website.

- **Additional Information:**
  - **Additional Information:** Any other relevant information about the product.
  - **Marketing Text:** Promotional and marketing descriptions for the product.

- **Export Formats:** Data can be exported in various formats including CSV, XLSX, JSON, JSONL, XML, and RSS for easy integration and analysis.

#### Output Data Sample
**Overview Table**
![Tesco Scraper Output](https://i.imgur.com/0fVDSMW.png)
**JSON**
```json
{
  "product_id": "310124535",
  "base_product_id": "90009500",
  "sku": "310124535",
  "gtin": "05000116126026",
  "brand_name": "BIRDS EYE",
  "name": "Birds Eye Green Cuisine Fishless Fingers 12 Pack 336G",
  "description": "Textured rice flake, coated in breadcrumbs, lightly fried. Open to UK residents aged 18+ only. Online registration & promotional product purchase required. 1 entry per email address and mobile number per day. Maximum 1 prize per email address, mobile number and household.  Purchase between 00:01 20/12/23 – 21:00 21/07/2024. Open for Entry: 00:01 03/01/2024 – 21:00 21/07/2024. Daily Prize Draw with 1 winner per day for 196 days. Total Prizes to be won: 196 x £200 Seasonal Experience Day Vouchers within the UK (Archery, Kayaking, Golf, Cycling, Shooting, Sports Climbing & Board Sports). All valid entries during promotional period will be eligible for entry into Final Draw on 22/07/2024 to win a trip to Paris (value to a min. of £3,000). Retain original itemised receipt dated within the Promotional Period and promotional product pack as proof of purchase. Visit www.green-cuisine.com/TeamGBWinSportPrizes to enter, for full T&Cs & Privacy Policy.. Promoter: Birds Eye Ltd., TW14 8HA. For a Sustainable Tomorrow. Making a difference with responsibly sourced and prepared food every day. BIRDSEYE.CO.UK/OUR-SUSTAINABLE-PATH",
  "price": 3.0,
  "currency": "GBP",
  "in_stock": true,
  "promotion": null,
  "unit": "G",
  "unit_price": 8.93,
  "unit_quantity": "336",
  "image_url": "https://digitalcontent.api.tesco.com/v2/media/ghs/9a487072-1c78-4b5f-ac5b-366379c2786e/5873296c-1f91-4c4d-bae0-b7a9f3b9239f.jpeg?h=225&w=225",
  "url": "https://www.tesco.com/groceries/en-GB/products/310124535",
  "buy_limit": 99,
  "buy_limit_message": "Max allowed is 99.",
  "is_new": false,
  "sale_type": "SingleProduct",
  "main_category": "Frozen Food",
  "sub_category": "Party Foods & Garlic Breads",
  "product_category": "Vegan Party Food",
  "product_type": "Frozen Vegan Party Food",
  "product_attributes": [
    "Vegan"
  ],
  "ingredients": [
    "Textured Rice Flake (40%)",
    "Wheat Flour",
    "Water",
    "Rapeseed Oil",
    "Wheat Gluten",
    "Potato Starch",
    "Natural Flavouring",
    "Salt",
    "Wheat Fibre",
    "Spices",
    "Yeast"
  ],
  "allergens": [
    "For allergens see ingredients in capital letters"
  ],
  "storage_instructions": [
    "Store in a freezer at -18°C or cooler."
  ],
  "usage_instructions": null,
  "nutrition": [
    {
      "Typical Values": "As Sold 100g Provides:"
    },
    {
      "Energy kJ": "1073kJ"
    },
    {
      "kcal": "257kcal"
    },
    {
      "Fat": "13g"
    },
    {
      "of which Saturates": "1.0g"
    },
    {
      "Carbohydrate": "26g"
    },
    {
      "of which Sugars": "1.7g"
    },
    {
      "Fibre": "2.0g"
    },
    {
      "Protein": "7.9g"
    },
    {
      "Salt": "1.3g"
    },
    {
      "A serving of 4 fishless fingers oven baked provides 1.5g α-Linolenic fatty acid": "-"
    },
    {
      "This pack contains 3 portions": "-"
    }
  ],
  "manufacturer": {
    "name": "Birds Eye Limited,",
    "adress": "Freepost ADM3939,London,SW1A 1YS.Birds Eye Ireland,",
    "email": null,
    "phone": "0800 33 22 77",
    "website": null
  },
  "additional_information": [
    "'Birds Eye' and 'the logo shape' are trademarks of Nomad Foods Europe Limited."
  ],
  "marketing_text": null
}
```

## 💬 Feedback and Support

**Your satisfaction** is **important** to us! Therefore we are constantly striving to enhance the performance of our Actors.

If you have any technical feedback or encounter any bugs with the Tesco UK Scraper, please create an issue in the Actor’s Issues tab on the Apify Console.

You can also contact us directly for custom integrations or project use cases at business@radeance.com.

Thank you and happy scraping!

[Try it out today for free on Apify! ](https://apify.com/radeance/tesco-scraper)