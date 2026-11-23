def knapsack_bottom_up(item_weights, item_values, bag_capacity):

    item_count = len(item_weights)

    table = [[0 for index in range(bag_capacity + 1)]
             for index in range(item_count + 1)]

    for item in range(1, item_count + 1):

        for current_capacity in range(1, bag_capacity + 1):

            current_weight = item_weights[item - 1]
            current_value = item_values[item - 1]

            if current_weight <= current_capacity:

                take_item = (
                    current_value +
                    table[item - 1][current_capacity - current_weight]
                )

                skip_item = table[item - 1][current_capacity]

                table[item][current_capacity] = max(
                    take_item,
                    skip_item
                )

            else:

                table[item][current_capacity] = table[item - 1][current_capacity]

    return table[item_count][bag_capacity]


item_weights = [2, 1, 3, 2]
item_values = [12, 10, 20, 15]

bag_capacity = 5

best_value = knapsack_bottom_up(
    item_weights,
    item_values,
    bag_capacity
)

print("Maximum value using Bottom-Up:",
      best_value)
