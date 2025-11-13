## Group Discussion Outcome

Our group decided on **Pokémon**. Pokémon was a very popular trading card series that started back in the 1990s and was created for both video games and trading cards.  

Below is a breakdown of the tables, with help from an AI assistant that summarized the database categories and categorical options. Our understanding is based on team effort, discussions, and each team member’s contribution to the database.

Our group discussed and decided what the options would be for the tables, and then divided the work among two team members to create the column names associated with those tables.  

Our database has **12 tables** with multiple columns. As a group, we didn’t face any major challenges. A few tables were eliminated because their columns duplicated existing ones in our database. One team member also pointed out some redundancy with a few foreign keys.

Our reasoning behind the database design was to maintain **simplicity** across all 12 tables. This is still a **work in progress** — a few columns still need to be eliminated. The reasoning behind our Pokémon columns is based on different models that allow both new and old users to have a platform to learn, buy, and engage.  

Ultimately, the goal is to allow users to **search, buy, or create more data** within our database, helping developers fine-tune, troubleshoot, and make the Pokémon database more **user-friendly**.

---

## AI Interpretation

This database models a **Pokémon card trading platform**.  

The central table, **`pokemon_card`**, stores card details such as name, health points, abilities, and links to related entities like `sets`, `energy_type`, `illustrators`, and `rarity`.

Cards can be listed for sale in the **`listings`** table, which includes pricing, order type, listing type, status, and timestamps.  

The **`users`** table holds buyer and seller information, connecting to **`transactions`**, which record completed sales with price, date, and user roles.  

Each transaction can include multiple **`transaction_items`**, specifying card quantities and individual prices.  

Supporting tables — **`status_types`**, **`order_types`**, and **`listing_type`** — define categories for listings and orders.

This structure ensures **normalized relationships** between users, cards, and transactions, allowing efficient management of Pokémon card trading data — from creation and illustration to listing, selling, and tracking transaction histories.
