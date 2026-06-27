Rule Area -                	Student-Facing Rule
Raw file-	                Do not overwrite raw_orders.xlsx. Create cleaned_orders.xlsx separately.
Missing region-             Fill as Unknown and flag in quality report.
Missing ship_mode-	        Fill as Unknown and flag in quality report.
Missing discount-	        Treat as 0 only if all other sales fields are valid; otherwise flag.
Discount-	                Flag negative discounts and unusually high discounts as invalid.
Cancelled/Failed/Refunded-	Do not include non-completed/failed/refunded records in completed-sales summaries.
Date sequence-	            Flag ship_date earlier than order_date.
Duplicates-	                Remove exact duplicate copies; flag conflicting duplicate order IDs.
Calculated fields-          Create calculated_sales, calculated_profit, profit_margin, shipping_delay_days, order_month, order_year, and data_quality_flag.
Documentation -          	Document cleaning decisions and assumptions in cleaning_log.md.
