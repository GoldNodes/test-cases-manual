# Test Cases – Analytics Dashboard

## Purpose:
To verify that the analytics dashboard displays accurate data, supports filtering, and exports data correctly.

| ID      | Title                                | Steps                                                                 | Expected Result                                           | Priority |
|---------|--------------------------------------|-----------------------------------------------------------------------|-----------------------------------------------------------|----------|
| TC-301  | Load analytics dashboard             | 1. Log in<br>2. Navigate to Analytics section                         | Dashboard loads with default date range and data          | High     |
| TC-302  | Apply date filter                    | 1. Open date picker<br>2. Select "Last 7 days"<br>3. Apply filter     | All graphs and metrics update accordingly                 | High     |
| TC-303  | Apply category or region filter      | 1. Select a category (e.g. "Product A")<br>2. Apply filter            | Dashboard displays data only for selected category         | Medium   |
| TC-304  | No data available                    | 1. Choose a date range with no activity                              | "No data available" message is displayed clearly          | Low      |
| TC-305  | Export data to CSV                   | 1. Click on "Export" button<br>2. Download CSV                        | File downloads correctly with expected data format         | Medium   |
| TC-306  | Data mismatch between UI and backend | 1. Open dashboard<br>2. Execute equivalent SQL manually               | Numbers on dashboard match SQL results                    | High     |
| TC-307  | Refresh dashboard                    | 1. Click refresh/reload on the dashboard page                         | All graphs reload without errors or duplication            | Medium   |
