import re

message = """
Please contact us at john@example.com or support@gmail.com.
You can also email admin@college.edu.in for further information.
"""

email_pattern = r'[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}'

email_list = re.findall(email_pattern, message)

print("Email addresses found:")

for address in email_list:
    print(address)
