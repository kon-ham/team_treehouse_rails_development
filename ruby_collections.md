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


