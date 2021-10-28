- Set a variable called last_item which uses the pop method to take the last item out of the grocery_list array.

    ```
    grocery_list = ["milk", "eggs", "bread", "ice cream", "carrots", "potatoes"]

    last_item = grocery_list.pop
    ```

- Set a variable called first_item which uses the shift method to take the first item out of the grocery_list array.

    ```
    grocery_list = ["milk", "eggs", "bread", "ice cream", "carrots", "potatoes"]

    last_item = grocery_list.pop

    first_item = grocery_list.shift
    ```

- Create a variable called grocery_item_1 which is a new hash.

    `grocery_item_1 = Hash.new`

- Create a key in the grocery_item_1 hash called "name" and set the value of that key to the string "milk".

    ```
    grocery_item_1 = Hash.new

    grocery_item_1["name"] = "milk"
    ```

- Using the has_key? method, check if the hash variable has a key called "calories". If it does, set a new variable called food to true.

    ```
    hash = { "name" => "Bread", "quantity" => 1, "calories" => 100 }

    food = hash.has_key?("calories")
    ```

- Using the has_value? method, check to see if the grocery_item hash has a value called "Bread". If it does, set a new key in the hash called "food" with the value of true.

    ```
    grocery_item = { "item" => "Bread", "quantity" => 1, "brand" => "Treehouse Bread Company" }

    grocery_item["food"] = true if grocery_item.has_value?("Bread")
    ```

- Use the values_at method on the grocery_item hash to get an array consisting of a single value: the value of the "item" key. Store the returned array in a variable named grocery_list.

    ```
    grocery_item = { "item" => "Bread", "quantity" => 1, "brand" => "Treehouse Bread Company" }

    grocery_item["food"] = true if grocery_item.has_value?("Bread")

    grocery_list = grocery_item.values_at("item")
    ```

- Using the merge method, create a hash named final_item that contains the grocery_item hash merged with the calories hash.

    ```
    grocery_item = { "item" => "Bread", "quantity" => 1, "brand" => "Treehouse Bread Company" }
    calories = { "calories" => 100 }

    final_item = grocery_item.merge(calories)
    ```

- Create a method named "create_shopping_list" that returns a hash. It does not need to ask for a name or get anything from standard input.

    ```
    def create_shopping_list
        Hash.new
    end
    ```

- Create a method called add_list_items that returns an array. It does not need to read from standard input.

    ```
    def add_list_items
        Array.new
    end
    ```

- Modify the "create_shopping_list" method to return a hash with the following keys and values:

    'title': A string with the value "Grocery List"
    'items': An empty array

    ```
    def create_shopping_list
        list_by_hash = { 'title' => 'Grocery List', 'items' => [] }
    end
    ```

- Let's add an item to our grocery list. We've set up a grocery_list hash that has an 'items' key with an empty array as its value. We've also created another hash and stored it in the grocery_item variable.

    Append the grocery_item hash to the empty array that's under the grocery_list hash's 'items' key.

    ```
    grocery_list = { 'title' => 'Grocery List', 'items' => [] }
    grocery_item = { 'title' => 'Bread', 'quantity' => 1 }

    grocery_list['items'] << grocery_item
    ```