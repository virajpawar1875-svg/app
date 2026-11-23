import csv
import json

with open("input.csv", "r", newline="") as source_file:
    csv_reader = csv.DictReader(source_file)
    records = list(csv_reader)

with open("output.json", "w") as target_file:
    json.dump(records, target_file, indent=4)

print("CSV data successfully converted to JSON.")
print("Output stored in output.json")
