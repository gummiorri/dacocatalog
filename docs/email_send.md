# EmailSend

Schema definition for the email_send table

## Fields

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `id` | string | Yes | Unique identifier for the email record (format: uuid) |
| `to_email` | string | Yes | Primary recipient email address (format: email) |
| `cc_email` | array(string) | No | List of CC recipient email addresses |
| `bcc_email` | array(string) | No | List of BCC recipient email addresses |
| `from_email` | string | Yes | Sender email address (format: email) |
| `subject` | string | Yes | Email subject line (maxLength: 255) |
| `body_text` | string | No | Plain text version of the email body |
| `body_html` | string | No | HTML version of the email body |
| `attachments` | array([Attachments](#Attachments)) | No | List of email attachments |
| `status` | string | Yes | Current status of the email (enum: `pending`, `queued`, `sent`, `failed`, `bounced`) |
| `provider` | string | No | Email service provider used to send the email |
| `provider_message_id` | string | No | Message ID returned by the email provider |
| `retry_count` | integer | No | Number of send retry attempts (minimum: 0) |
| `error_message` | string | No | Error message if sending failed |
| `sent_at` | string | No | Timestamp when the email was successfully sent (format: date-time) |
| `created_at` | string | Yes | Record creation timestamp (format: date-time) |
| `updated_at` | string | No | Record last update timestamp (format: date-time) |


---

## Attachments

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `file_name` | string | Yes |  |
| `content_type` | string | Yes |  |
| `file_size` | integer | Yes |  (minimum: 0) |
| `file_url` | string | No |  (format: uri) |

