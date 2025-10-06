**Cake Order Inquiry Automation**

This workflow takes orders from google sheets and categorizes orders into high or low priority based on their budget. If an order is labeled High Priority, a email will be sent with the customer's information.

We used make.com to create this automation. The modules we used were as follows:
- Google sheets - watch new rows
- Test parser - match pattern
- Tools - set variable
- Router
    - if above 500 - google sheets updates row to high priority
    - if below 500 - google sheets updates row to low priority
- if high priority - Gmail sends an email
