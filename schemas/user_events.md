# UserEvents

## Fields

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `dt` | timestamp | Yes |  |
| `game_id` | integer | Yes |  |
| `game_var_id` | integer | Yes |  |
| `trns_tp` | integer | Yes |  |
| `acc_id` | integer | No |  |
| `year_` | integer | No |  |
| `bd_id` | integer | No |  |
| `ret_id` | integer | No |  |
| `parent_ret_id` | integer | No |  |
| `oper_id` | integer | No |  |
| `term_id` | long | No |  |
| `empl_id` | string | No |  |
| `external_retailer_id` | integer | No |  |
| `played_draw` | integer | No |  |
| `product_id` | integer | No |  |
| `coupons` | long | No |  |
| `coupons_gm_var` | long | No |  |
| `cols` | long | No |  |
| `gross_amn` | decimal(20,8) | No |  |
| `net_amn` | decimal(20,8) | No |  |
| `refund_amn` | decimal(20,8) | No |  |
| `tax_amn` | decimal(20,8) | No |  |
| `bonus_amn` | decimal(20,8) | No |  |
| `disc_amn` | decimal(20,8) | No |  |
| `comm_amn` | decimal(20,8) | No |  |
| `fee_amn` | decimal(20,8) | No |  |
| `refund_coupons` | long | No |  |
| `refund_fee_cpns` | long | No |  |
| `_record_id` | string | No | Unique identifier for the record. |
| `_load_date` | timestamp | No | Timestamp indicating when the record was loaded. |
| `_trace` | [Trace](#Trace) | No | Tracking metadata for lineage and traceability. |
| `_dq_issue` | boolean | No | Flag indicating if the record has a data quality issue. |
| `_dq_issue_reason` | array(string) | No | Reason for the data quality issue. |
| `_silver_ts` | timestamp | No | Timestamp indicating when the record was written. |


---

## Trace

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `_record_id` | string | No |  |
| `_source_table` | string | No |  |

