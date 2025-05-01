# Test Cases – Checkout Process (E-commerce)

## Purpose:
To verify the complete order flow from cart to payment confirmation.

| ID      | Title                              | Steps                                               | Expected Result                              | Priority |
|---------|------------------------------------|-----------------------------------------------------|----------------------------------------------|----------|
| TC-101  | Successful checkout with valid data| Add item → go to cart → checkout → fill details → pay | Order confirmed with summary screen         | High     |
| TC-102  | Checkout with empty cart           | Go to cart → Click checkout                         | Error: "Cart is empty"                        | Medium   |
| TC-103  | Invalid card during payment        | Add item → checkout → enter expired card            | Payment declined, error shown                | High     |
| TC-104  | Missing shipping address fields    | Leave zip code empty → click pay                    | Validation error near zip field              | Medium   |
| TC-105  | Cancel checkout mid-process        | Start checkout → click back or close window         | User returned to cart without errors         | Low      |
